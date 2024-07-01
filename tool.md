## Analytic Tool

[Reference](https://derivatives.hcommons.org/2021/07/)

### Implied Volatility Calculator

An implied volatility is the volatility implied by the market price of an option based on the Black-Scholes option pricing model. Given an option price, the model can calculate implied volatility.

The term structures of implied volatilities which provide indications of the market’s near- and long-term uncertainty about future short- and long-term swap rates. A crucial property of the implied volatility surface is the absence of arbitrage.

Vol skew or smile pattern is directly related to the conditional non-normality of the underlying return risk-neutral distribution. In particular, a smile reflects fat tails in the return distribution whereas a skew indicates return distribution asymmetry.


References:
 
[Link](/ToolEqVol-1.pdf)

[OSF vol](https://osf.io/xp5s6/download)

[Zenodo vol](https://zenodo.org/record/5207836/files/ToolEqVol-1.pdf)

[Github vol](https://github.com/cfrm17/ImpliedVolCalculator)




### Forward Dividend Calculator

Forward dividends are also called expected future dividends, or projected dividend, or implied dividends. They are critical for valuing any equity products. In other words, the key factor for pricing equity products is to correctly calculate equity forward taking all dividends into account. The stock price is adjusted by dividends over ex-dividend dates. 

An equity model must account for all the dividend payments between valuation date and the option maturity date. Those dividends are forward (or future or projected or implied) dividends. FinPricing provides tools for computing forward dividends based on market prices. Those dividends will allow you to match market quotes, expectations, and forecasting. By using the implied forward dividends, you can archive risk neutral or no arbitrage valuation.

Dividends tend to reduce the price of a stock on ex-dividend date by the amount of the dividend. All the equity models need to be adjusted to allow for the payout of dividends. There are three types of dividends: constant dividend yield, term structure of dividend yields, and term structure of discrete dividends.


References:
 
[Link](/ToolEqDiv-2.pdf)

[OSF Dividend](https://osf.io/hrtnc/download)

[Zenodo Dividend](https://zenodo.org/record/5233752/files/ToolEqDiv-2.pdf)

[Github Dividend](https://github.com/cfrm17/forwardDiv)


### CNY Curve

The market standard is to generate the base curve using market quotes and a bootstrap method. FX forward spreads are used as quote inputs to generate FX curve and combined with the CNY zero curve to derive the necessary 
quoting currency.

[CNY Curve Introduction](cny.md)


### Volatility Adjustment Factors

The three volatility adjustment factors reflect the average level of High/Medium/Low issuer-specific spread risks, which may not be granular enough (e.g. some issuers may have extremely high or low spread volatilities 
which is different from the average level). This may lead to biased exposure result so we regard this uncertainty to be an observation.

[Volatility Adjustment Introduction](volAdj.md)
