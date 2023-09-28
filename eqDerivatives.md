## Equity Derivatives


### Asian Basket Options with Individually Capped Returns

We compute the payoff M times and then take the average. If M is large enough, then these average approaches the expectation we are looking for (an application of the Strong Law of Large Numbers). Alongside we also compute the statistical standard error. Note that if the valuation date is later than an averaging date, then on that date the realized price must be used in the computation of the payoffs. The sensitivities are computed using finite differencing with path recycling. 

References: 

[Zenodo Asian Basket pdf](https://zenodo.org/record/7474285/files/AsianBasket.pdf)

[Zenodo Asian Basket](https://zenodo.org/record/7474285)

[Github Asian Basket](https://github.com/cfrm17/asianBasket)



### Cross Currency Option 

Since there are two sources of uncertainties involved in the option, one resulting from underlying price changes and the other resulting from changes in the exchange rate, this option is non-quanto.  The holder of the option bears the risk caused by the fluctuation of the exchange rate between the underlying currency and the payoff currency.  

As to the discrete dividends, since they are a riskless component in the stock price dynamic, the spot stock price should be reduced by the present value of all the dividends during the life of the option.  Let   be the current value date.   Taking the predicted discrete dividends of the underlying stock into account, the translated stock price at time zero is given 

References:


[Github XCCY Option](https://github.com/cfrm17/xccyOption)


### Average Rate (Asian) Option 

These include: Monte Carlo simulation, numerical inversion of the Laplace transformation of the Asian option price derived by Geman and Yor (1993), alternative PDE techniques suggested by Rogers and Shi (1995), and various approximations (for instance, Turnbull and Wakeman (1991), and Curran (1994)). Numerical inversion of the Laplace transform or PDE techniques of Rogers and Shi tend to give inaccurate results for cases of short maturities or small volatilities. Monte Carlo simulation always works well, but it can be computationally inefficient. 

References:

[Zenodo Asian Option pdf](https://zenodo.org/record/7478480/files/AverageRateOption.pdf)

[Zenodo Asian Option](https://zenodo.org/record/7478480)

[Zenodo Asian Option](https://github.com/cfrm17/averageRateOption)


### Multiple-Underlying Capped Accumulated Return Call Option

A pricing model is presented for capped-accumulated-return-call (CARC) with multiple underlyings. At each reset date, a weighted stock price is calculated.  These weighted stock prices are used to compute returns.

References:

[Github Multi CARC](https://github.com/cfrm17/multiCarc)


### Capped Accumulated Return Call Option with Two Way Return and Splitting Payoff

An enhanced Quasi-Monte Carlo method is employed to evaluation this feature of CARC.  In this method, Sobol sequence in conjunction with Brownian Bridge path generation approach is applied.  In this transaction,   is  ,   is 0.12,   is 0.147, and the notional principal is USD 100.  Only the term structure of at-the-money volatility is used in calculation, i.e., volatility skew is NOT applied.

References:

[Zenodo Two Way CARC pdf](https://zenodo.org/record/7480149/files/TwoWayCarc.pdf)

[Zenodo Two Way CARC](https://zenodo.org/record/7480149)

[Github Two Way CARC](https://github.com/cfrm17/twoWayCarc)


### Capped Accumulated Return Call with Volatility Surface

A new representation of the volatility skew is provided.  To use this new representation, the user must input “STRIKE_REPRESENTATION   PERCENTAGE” in the token file.  Then, the ATM strike is always assumed to be 100.  The first quantity in the volatility skew still signifies the stock price when the volatility skew was built.  

The model will interpret this skew as follows.  At the time 1 year from the date when the volatility skew was built, the 10% ITM volatility is 0.4, with the strike level being 90*1050/100=945.  The ATM volatility is 0.38 with the strike level being 1050*100/100=1050.  The 10% OTM volatility is 0.36 with the strike level being 110*1050/100=1155.  At the time 2.0 years, a similar interpretation can be obtained.

References:

[Zenodo Two Way CARC pdf](https://zenodo.org/record/7487163/files/CarcVolSurface.pdf)

[Zenodo Two Way CARC](https://zenodo.org/record/7487163)

[Github Two Way CARC](https://github.com/cfrm17/carcVol)


### Capped Accumulated Return Call Valuation with Lock-In Feature

A Monte Carlo (Gaussian MC and Quasi MC) pricing model is presented for the product named capped-accumulated-return-call (CARC) with lock in feature.  

References:

[Zenodo Lockin CARC pdf](https://zenodo.org/record/7487196/files/CARCLockIn.pdf)

[Zenodo Lockin CARC](https://zenodo.org/record/7487196)

[Github Lockin CARC](https://github.com/cfrm17/carcLockIn)


### Capped Accumulated Return Call with Flexible Return

A Monte Carlo (Monte Carlo, MC, and Quasi Monte Carlo, QMC) pricing model is presented for a new variation on the product named capped-accumulated-return-call (CARC): CARC with pick and choose the return period. User specifies the dates where equity returns are to be calculated and then used in the final payoff.

References:

[Zenodo Flexible Return CARC pdf](https://zenodo.org/record/7487231/files/CarcFlexibleReturn.pdf)

[Zenodo Flexible Return CARC](https://zenodo.org/record/7487231)

[Github Flexible Return CARC](https://github.com/cfrm17/carcFlexibleReturn)


### Futures Fair Value Adjustment

We recommend that the new method be approved in order to determine the fair value of futures contracts for index arbitrage. This is important because the current method undervalues predominantly short futures positions creating erosion of P&L over the life of the contract.

References:

[Zenodo Fair Value Adjustment pdf](https://zenodo.org/record/7526407/files/FairValueAdjustment.pdf)

[Zenodo Fair Value Adjustment](https://zenodo.org/record/7526407)

[Github Fair Value Adjustment](https://github.com/cfrm17/fairValueAdjustment)


### Expiration Price Option 

An Expiration Price Option (EPO) is an option with a knock-out feature. At any time, if the option value is equal or less than a specified barrier price, the writer of the option will provide notification to the option holder. The option holder can either

•	Pay an additional premium to prevent the option from knocking-out. The additional premium is equal to the difference between initial premium and the option value at the time of notification.
•	Pay nothing to allow the option to be knocked out. The writer pays the option holder an amount equal to

References:

[Zenodo Expiration Price Option pdf](https://zenodo.org/record/7526459/files/EpoModel.pdf)

[Zenodo Expiration Price Option](https://zenodo.org/record/7526459)

[Github Expiration Price Option](https://github.com/cfrm17/epoModel)


### Equity for Float Swap 

For our equity-for-float swap, two swap values are calculated: economic and replacement.  The economic value is the value of the swap to one party, while the replacement value is the dollars received/paid to offset the swap to a third party.

When we say selling a swap, we pay the return on equity and receive Libor plus a spread.  The economic value of the swap is decomposed into 4 parts: current equity (CE), future equity (FE), current interest rate (CI), and future interest rate (FI).  The value of CE is the present value of the capital gains and dividends of the underlying stock portfolio between the beginning of the first equity reset date   and the end of the first equity reset date  .  

References:

[Zenodo Equity Float Swap pdf](https://zenodo.org/record/7526526/files/equityForFloatSwap.pdf)

[Zenodo Equity Float Swap](https://zenodo.org/record/7526526)

[Github Equity Float Swap](https://github.com/cfrm17/equityForFloatSwap)


### Equity Forward with Settle Date Lag and Dividend Percentage

Two new features are added in the equity forward pricing model.  One feature is settle date lag, which is introduced to match market conventions as forward contracts are sometimes settled with a delay.  The other feature is dividend percentage, which allows the model user to use part of the real dividend for calculation.

Suppose the initial trade date is set to time zero, the maturity of the forward is T.  If there is a delay of   for the forward contract to be effective, and a delay of   for the contract to be settled, the forward price is calculated

References:

[Zenodo Equity Feature Forward pdf](https://zenodo.org/record/7526566/files/specialEquityForward.pdf)

[Zenodo Equity Feature Forward](https://zenodo.org/record/7526566)

[Github Equity Feature Forward](https://github.com/cfrm17/specialEquityForward)

### Equity Futures Contract 

The output of the model is the mark to market value of such a contract, that is, the Equity Futures price less the strike (if long position).

References:

[Zenodo Equity Futures pdf](https://zenodo.org/record/7539063/files/equityFutures.pdf)

[Zenodo Equity Futures](https://zenodo.org/record/7539063)

[Github Equity Futures](https://github.com/cfrm17/equityFutures)


### Binary Return Note 

The three deals used differ by the stock correlation matrix (the last two of them are extreme cases), as this is one the most important risk factor (multi-path generation starts with a multi-dimensional Brownian motion whose correlation matrix is our stock correlation matrix).
In order to measure the difference, we use the following measure:

Considering the Monte Carlo nature of the model, the differences for Delta and Vega are reasonably small for all test cases. As expected we notice big relative differences in Gamma. This happens typically when the magnitude of Gamma is small. Middle Office should independently study Greek convergence. Gamma should be monitored too.

References:

[Zenodo Binary Return pdf](https://zenodo.org/record/7539127/files/binaryReturn.pdf)

[Zenodo Binary Return](https://zenodo.org/record/7539127)

[Github Binary Return](https://github.com/cfrm17/binaryReturn)


### Reverse Convertible 

As this payoff involves continuous barriers, the expectation of this payoff can be calculated using a version of conditional Monte Carlo method. Biased upper and lower estimator bounds plus a biased price placed between these bounds (using a stock event independence assumption) are proposed. We describe this method below.

Based on above payoff re-write, the price of a Reverse Convertible on single asset is the difference between the price of a Cash-or-Nothing European Digital Call with rebate C and a Down and In Put with strike K , B barrier strike, notional N K , to which the notional is added. Accordingly, one has a closed-form pricing available. 

References:

[Zenodo Reverse Convertible pdf](https://zenodo.org/record/7539157/files/reverseConvertible.pdf)

[Zenodo Reverse Convertible](https://zenodo.org/record/7539157)

[Github Reverse Convertible](https://github.com/cfrm17/reverseConvertibleModel)


### 401K Stable Value Protection 

The stable value model is aimed at pricing the value of providing value protection on a portfolio consisting of fixed income instruments.  The protection provided by the stable value contract is written on any shortfall between the market value of the fund and a defined “book value” which exists when redemptions or withdrawals from the fund are made.

The book value of the fund is computed as a function of the “crediting rate”, which itself is a function of previous market and book values as well as the equity and/or fixed income indices that indicate the market value of the fund.

References:

[Zenodo 401K pdf](https://zenodo.org/record/7542073/files/401kFund.pdf)

[Zenodo 401K](https://zenodo.org/record/7542073)

[Github 401K](https://github.com/cfrm17/401kFund)


