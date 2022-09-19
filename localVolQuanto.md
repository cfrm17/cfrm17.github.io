
### Local Volatility Model for Callables

We review a model for computing the price, in the domestic currency, of European standard call and put options on an underlying foreign equity (stock or index) with tenor of up to 7 years. 
The function implements a local volatility based pricing method.

The equity price process satisfies a risk-neutral stochastic differential equation (SDE) when where are no dividend payments. Let St denote the equity price at time t. We assume that the 
process satisfies a SDE of the form under the domestic risk-neutral probability measure

We note that the volatility σ depends only on time and on the instantaneous value of the state variable S, but does not explicitly depend on W.

Consider the calibration of the local volatility function based on market option prices or, equivalently, market Black’s implied volatilities. If there exists a smooth surface of either 
option price or implied volatility as a function of option strike and maturity, then this surface uniquely determines the local volatility function.

Moreover, an explicit expressions for local volatility is provided. For example, if C denotes the price of a call option on a non-dividend paying stock, with a constant risk-free interest rate,

Local volatility model can also be applied to value callable exotic notes. Callable option is more volatile as callable events make the remaining part of the trade potentially be cancelled 
as a result of a trigger condition or an exercise option. In general, local volatility model is very useful tool for pricing equity derivatives.




References:

[pdf](https://osf.io/74s83/downloand)

[wiki](https://osf.io/cms8h/wiki/home/)





