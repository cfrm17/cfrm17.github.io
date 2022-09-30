
### American Bond Option Valuation

A valuation model is presented for pricing an American style call option on the yield of Treasury bond. The payoff is positive if the yield exceeds a predetermined strike level. The model assumes the yield of an American Treasury bond to be a log-normally distributed stochastic process and uses Monte-Carlo simulation to price the deal as a European call option. 

At the time of maturity of the option the yield distribution is taken as y = yf exp(-0.52T + W), where yf  is the bond’s forward yield (by the time T, which is the option tenor). The payoff is averaged over this distribution and discounted to the trade date. 

The yield to maturity of a bond is computed as https://finpricing.com/lib/FiZeroBond.html

The model builds a trinomial tree for the yield process to price the deal as an American option. The time slices of the tree are evenly spaced. Node transition probabilities and the time interval between slices are determined by matching the first four moments of the underlying Brownian motion. The option is priced using the backward induction.

Since the considered option is analogous to an American call option on a stock without dividends, its pricing as a European call is justified by the arbitrage argument: the value of today’s exercise is S-X, while the present value of the exercise at  maturity is  at least S-Xexp(-rT), which is higher. This approach is also verified by our testing.

Since the term of the option is less than half of year,  which is much less than the term of the underlying bond, it also acceptable to treat the bond’s yield as a lognormally distributed stochastic process with a constant volatility.

The payoff of the option is a discontinuous function of yield, which technically represents the primary security. As a result, the delta is not defined for the intrinsic case, and it is poorly defined for small volatilities. Therefore, the use of delta is not recommended for volatilities less than 5% or for time to maturity less than 10 days.

Since the underlying security (“stock”) is represented by a discrete grid, the payoff function (such as S-X>0 for the call, solid line in the Fig. 1) is also distorted and represented by a step–wise line (dashed line in Fig. 1). The option price is roughly determined by the area under both the payoff function and the Gaussian curve. One can see from the figure that relative error introduced by the discretization may be the largest for medium variance of the Gaussian distribution.

The model assumes the yield of an American Treasury bond to be a log-normally distributed stochastic process and uses Monte-Carlo simulation to price the deal as a European call option.

The contract is a binding agreement between two parties as to the terms of the transaction to which this contract relates. In addition, two parties agree to use all reasonable efforts promptly to negotiate, execute and deliver an agreement in the form of the ISDA Master Agreement, with such modifications as we in good faith agree.

On the cash settlement payment date, the seller shall pay the buyer the cash settlement amount provided the settlement rate is equal to or greater than the strike rate.

References:

[pdf](https://osf.io/q6ut7/download)

[list](https://finpricing.com/FinPricing-ProductBrochure.pdf)





