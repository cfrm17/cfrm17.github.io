
### CMS Spread Option Valuation

A constant maturity swap (CMS) spread option makes payments based on a bounded spread between two index rates (e.g., a GBP CMS rate and a EURO CMS rate).  The GBP CMS rate is calculated from a 15 year swap with semi-annual, upfront payments, while the EURO CMS rate is based on a 15 year swap with annual, upfront payments. 

Let
•	  be a CMS rate fixing time,
•	  be a payment time,
•	  and   respectively denote the GBP and EURO CMS rates at the fixing time,
•	  be a CMS rate spread.

Then, at time  , the buyer must pay a spread,  , bounded below and above by 0% and 10% respectively, multiplied by the accrual period,  ;  formally the payoff is given 

We assume that both the forward GBP and EURO CMS rates follow geometric Brownian motion under their respective  -forward measures.  Here respective initial forward CMS rates are calculated.  The forward rates are then convexity adjusted from respective parallel bonds specified using

•	the same payment times as the underlying CMS,
•	coupon equal to the forward CMS rate,
•	initial bond yield equal to the forward CMS rate.

From the above the correlation, under foreign T-forward measure, between the Brownian motions respectively driving the foreign bond yield and GBP swap rate processes constrains the correlation between the Brownian motions driving the Euro bond yield and forward GBP CMS rate processes under domestic T-forward measure.  Bond yield is computed from bond price (see https://finpricing.com/lib/FiZeroBond.html).

To evaluate the expression above, we require the SDE followed by the forward exchange rate process under domestic T-forward measure.  This is derived by changing measure from foreign  -forward measure, to domestic risk-neutral measure, to domestic  -forward measure.

For more pricing accuracy, the forward price of the Euro denominated zero-coupon bond, used in the calculation of the delayed payment adjustment, should then also be based on these adjusted discount factors.

The price is given by its expected value under the EURO (domestic) T-forward measure. The benchmark pricing method is based on Gauss-Hermite integration of the resulting three-dimensional integral over the true joint density for the respective CMS rates and the EURO zero-coupon bond yield-to-maturity.

References:

[pdf](https://osf.io/9db5u/download)

[Zenodo broker strange pdf](https://zenodo.org/record/7317278/files/BrokerStrangleAlgorithm.pdf)

[Zenodo broker strange](https://zenodo.org/record/7317278)

[Zenodo fix barrier pdf](https://zenodo.org/record/7320191/files/SingleFixingBarrier.pdf)

[Zenodo fix barrier](https://zenodo.org/record/7320191)

