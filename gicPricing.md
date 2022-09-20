
### GIC Valuation

Guaranteed investment certificate (GIC) is a financial instrument that offers a return based on a corresponding GIC rate and the performance of a basket of certain stock and bond market indices. A bond can be valued as https://finpricing.com/lib/FiBond.html

To determine the rate of return, the percentage change in each index level from the initial level is calculated.  Here the initial level is set two days after purchase, while the final level is set to the arithmetic average of the last 11 month-ending index levels and the level one day prior to maturity.  

The rate of return is then given by a weighted sum of the GIC rate and the percentage change in each index level described above, but bounded below by a minimum guaranteed interest rate.  At maturity, the GIC holder receives the invested principal plus the principal times this rate of return.  

The payoff at maturity from a GIC can be shown equal to the invested principal plus these principal times the sum of the minimum guaranteed interest rate and the payoff from a European call option on the arithmetic average of a basket price at the 12 points above, where the basket price is given by a weighted sum of the index levels above.  

We consider the pricing of this call option.  We assume that each of the underlying stock and bond market indices in the basket follows geometric Brownian motion with drift under their respective risk neutral probability measures.  Each index process is then expressed under the Canadian risk neutral probability measure by means of a corresponding quanto adjustment.  

Observe that the basket price arithmetic average is not lognormally distributed.  Corporate Treasury’s approach towards pricing the call option, then, is to approximate the basket price arithmetic average using a shifted lognormal random variable.  Here the defining parameters for the approximating random variable are uniquely determined by matching the first three moments of the basket price arithmetic average.  The call option price is then given analytically.

The payoff at maturity from a GIC can be shown equal to the invested principal plus this principal times the sum of the minimum guaranteed interest rate and the payoff from a European call option on the arithmetic average of the basket price, where the basket price is given by a weighted sum of the index levels.

We assume that each of the basket’s underlying stock and bond market indices follows geometric Brownian motion with drift under its respective risk neutral probability measure. Each index process is then expressed under the Canadian risk neutral probability measure by means of a corresponding quanto adjustment.

We approximate the basket price arithmetic average by a shifted lognormal random variable. Here the defining parameters for the approximating random variable are uniquely determined by matching the true, first three moments of the basket price arithmetic average. The European call option price is then given analytically by a Black Scholes type of formula.

References:

[pdf](https://osf.io/tgd82/download)

[wiki](https://osf.io/9rpb3/wiki/home/)





