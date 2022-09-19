
### Forward Starting Option Valuation

Forward start option is an option whose strike will be determined at some later date. Unlike a standard option, the strike price is not fully determined until an intermediate date before expiration. 
Cliquet option consists of a series of forward start options. 

Employee stock option is a forward start option. The strike price is not fixed when the employee began to work. Instead, he is promised that he will receive stock option at periodic dates in the future. 
The strikes of employee stock options are unknown for now, but will be set to be at the money on later dates. 

A model is presented for pricing European exercise, forward starting options on an underlying equity. The payoff at maturity T is given.

Note that the volatility depends only on time and on the instantaneous value of the state variable S, but does not explicitly depend on Wt.
In practice, option price or implied volatility surfaces are available at points on a relatively sparse grid of strike and tenor pairs. Using analytical expressions to determine the local volatility 
function then likely yields inaccurate results due to the numerical instability from calculating first, and especially, second derivatives.

This difficulty can be avoided by approximating the SDE dynamics via a partial differential equation (PDE).

Volatility surface input can be specified according to the following three respective representations:

	Skew-tail parametric model (i.e., the surface is fully specified by three parameters, which are respectively called “skew”, “tail”, and “anchor”),
	Polynomial parametric model (i.e., specified by coefficients of polynomial in strike and 1/√tenor and
	Implied volatility grid.

The valuation requires two interest rate curve inputs. One curve, called the “hedge curve”, is specified by a list of n term and continuously compounded zero rate pairs and is intended for use in 
computing forward equity values.

The other, called the “discount curve, is specified by a list of m term and continuously compounded zero rate pairs, and is intended for use in calculating discount factors,

By using two different interest rate curves, we can facilitate certain (e.g., quanto) adjustments to interest rates.

To calculate Delta and Gamma, one needs to shift the equity spot price and computes the option price over a grid of strike and tenor pairs. This computation requires the implied volatility at each 
grid point based on the shifted spot value.




References:

[pdf](https://osf.io/37fbt/download)

[wiki](https://osf.io/x29t8/wiki/home/)





