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

[Zenodo XCCY Option pdf](https://zenodo.org/record/7474447/files/CrossCcyOption.pdf)

[Zenodo XCCY Option](https://zenodo.org/record/7474447)

[Github XCCY Option](https://github.com/cfrm17/xccyOption)


### Average Rate (Asian) Option 

These include: Monte Carlo simulation, numerical inversion of the Laplace transformation of the Asian option price derived by Geman and Yor (1993), alternative PDE techniques suggested by Rogers and Shi (1995), and various approximations (for instance, Turnbull and Wakeman (1991), and Curran (1994)). Numerical inversion of the Laplace transform or PDE techniques of Rogers and Shi tend to give inaccurate results for cases of short maturities or small volatilities. Monte Carlo simulation always works well, but it can be computationally inefficient. 

References:

[Zenodo Asian Option pdf](https://zenodo.org/record/7478480/files/AverageRateOption.pdf)

[Zenodo Asian Option](https://zenodo.org/record/7478480)

[Zenodo Asian Option](https://github.com/cfrm17/averageRateOption)


### Multiple-Underlying Capped Accumulated Return Call Option

A pricing model is presented for capped-accumulated-return-call (CARC) with multiple underlyings. At each reset date, a weighted stock price is calculated.  These weighted stock prices are used to compute returns.

[Zenodo Multi CARC pdf](https://zenodo.org/record/7480124/files/MultiCarc.pdf)

[Zenodo Multi CARC](https://zenodo.org/record/7480124)

[Github Multi CARC](https://github.com/cfrm17/multiCarc)


### Capped Accumulated Return Call Option with Two Way Return and Splitting Payoff

An enhanced Quasi-Monte Carlo method is employed to evaluation this feature of CARC.  In this method, Sobol sequence in conjunction with Brownian Bridge path generation approach is applied.  In this transaction,   is  ,   is 0.12,   is 0.147, and the notional principal is USD 100.  Only the term structure of at-the-money volatility is used in calculation, i.e., volatility skew is NOT applied.

[Zenodo Two Way CARC pdf](https://zenodo.org/record/7480149/files/TwoWayCarc.pdf)

[Zenodo Two Way CARC](https://zenodo.org/record/7480149)

[Github Two Way CARC](https://github.com/cfrm17/twoWayCarc)




