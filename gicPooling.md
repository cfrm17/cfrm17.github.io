
### GIC Valuation

Guaranteed investment certificate (GIC) is a financial instrument that offers a return based on a corresponding GIC rate and the performance of a basket of certain stock and bond market indices.

To determine the rate of return, the percentage change in each index level from the initial level is calculated.  Here the initial level is set two days after purchase, while the final level is set to the arithmetic average of the last 11 month-ending index levels and the level one day prior to maturity.  

The rate of return is then given by a weighted sum of the GIC rate and the percentage change in each index level described above, but bounded below by a minimum guaranteed interest rate.  At maturity, the GIC holder receives the invested principal plus the principal times this rate of return.  

The payoff at maturity from a GIC can be shown equal to the invested principal plus these principal times the sum of the minimum guaranteed interest rate and the payoff from a European call option on the arithmetic average of a basket price at the 12 points above, where the basket price is given by a weighted sum of the index levels above.  

We consider the pricing of this call option.  We assume that each of the underlying stock and bond market indices in the basket follows geometric Brownian motion with drift under their respective risk neutral probability measures.  Each index process is then expressed under the Canadian risk neutral probability measure by means of a corresponding quanto adjustment.  

Observe that the basket price arithmetic average is not lognormally distributed.  Corporate Treasury’s approach towards pricing the call option, then, is to approximate the basket price arithmetic average using a shifted lognormal random variable.  Here the defining parameters for the approximating random variable are uniquely determined by matching the first three moments of the basket price arithmetic average.  The call option price is then given analytically.

The GIC specification includes
•	the maturity (either 3 or 5 years),
•	initial levels for the five indices above, set to the respective index closing level on the second business day after the date of purchase, 
•	twelve averaging times, respectively set to the last business day in each of the eleven months that precede the month in which the GIC matures and the business day that immediately precedes the maturity date,
•	a GIC interest rate with corresponding compounding frequency, and
•	a participation rate, which is the percentage of the net return on the index components.

For each index, let

*	  denote the index closing  level,
*	  denote the corresponding weight,
*	IIL denote the initial index level, 




References:

[pdf](https://osf.io/atyb9/download)

[wiki](https://osf.io/4kwbp/wiki/home/)





