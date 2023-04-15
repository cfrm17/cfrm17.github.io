
### Callable Inverse Swap Valuation

A Callable Inverse Floating Rate Swap is a forward swap agreement with an option of canceling the swap each year starting from several years in future. The deal is priced with a two factor Black-Karasinski model.

The Black-Karasinski class of models assumes the short term interest rates to be log-normally distributed. The spreadsheet mode used for the deal pricing has a hard-coded term structure of the mean reversion and volatility parameters, constructed as Chebyshev polynomials. 

The calibration procedure takes only an interest rate curve as input (ignoring volatility surfaces) and results in adjusting the “alpha” parameter of the model. To test the calculations over a range of parameters, we used  the “piece-wise constant parametrization” mode. 

The Black-Karasinski model is set with zero mean reversion. The zero mean reversion makes it easy to perform simulations on a recombining binomial tree.

To provide the ability to control interest rates for our testing, the interest rate curve was constructed as a flat yield curve at a prescribed yield level. One set of the tests used the interest rate term structure as generated.

A few tests of internal consistency of the model raise some concerns. The results of symmetry tests cannot be accounted for by numerical truncation errors. 

Fortunately, these discrepancies are not important for the deal under consideration. The reason is that the price dynamics that affect the deal is driven by essentially one factor process.  The history of tests of one factor driven processes supports the validity of pricing. 

One trade example is shown as: Starting January 9, 1999, part onw pays party tow 5% on the notional of 15,000,000 DEM annually for the years 1999 through 2004. For the following five years party one pays annually the floating rate calculated as r - (2 * 12 month DEM LIBOR * 365/360) floored at 0, where r is set to 12.5% for year 6, 13.4% for year 7, 14.3% for year 8, 15.2% for year 9, and 16.1% for year 10.

Party one has the right to cancel the swap on the annual payment date, starting on January 9, 2004, and every year thereafter. Day counting convention for the payment is 30/360. In exchange, party two pays party one 6 month DEM LIBOR – 8 basis points on the same notional semiannually based on the ACT/360 day counting convention.

References:

[osf pdf](https://osf.io/9jyh8/download)

[Zenodo reciprocal average pdf](https://zenodo.org/record/7317169/files/ReciprocalAverageForward.pdf)

[Zenodo reciprocal average](https://zenodo.org/record/7317169)

[Zenodo reciprocal average](https://zenodo.org/record/7317169)

