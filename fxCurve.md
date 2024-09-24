
### Fx Implied Yield Curve


An FX implied yield curve is derived using the arbitrage-free relationship between forward FX rates and discount rates of the two currencies.
Market standard is to use FX forward spreads as quote inputs to generate FX implied yieldcurve and combined with the base zero curve derive 
necessary quoting currency.

The bid and ask rates of the FX quote are used to identify the quote side. Note, using BID and ASK spreads as inputs can result in unrealistic 
spreads on the resulting interest rates. For this reason it is preferred to use mid rates and only add a spread when making a trade. In the 
setup of the testing environment, bid, ask and mid had the same value, therefore the mid rates were used for testing. 

To generate FX curves, the FX Points Generator algorithm is used. It generates curve dates, uses FX forward spreads as quote inputs and adjusts 
points for O/N and T/N market conventions. The generator is very simple, because the FX swap points are the forward FX points for dates after 
the spot date

For markets in which the spot date is two business days from today, find the FX swap rate for exchange today by summing the O/N and the T/N 
quotes; if the spot date is only one business day, today’s points are given by the O/N quote alone.

The model uses market standard methodology. Based on the calculations,  the FX derived curve construction is accurate when deriving the quoting 
currency from the USD zero curve and FX forward spreads.


References:

[Archive hitting probability](https://ia600203.us.archive.org/31/items/barrierProbabilityNew/barrierProbabilityNew.pdf)

[Hcommons hitting probability](https://hcommons.org/deposits/download/hc:63250/CONTENT/barrierprobability.pdf/)

[Hcommons hitting probability Introduction](https://hcommons.org/deposits/item/hc:63249/)

[Science hitting probability Introduction](https://science-media.org/presentation/652)







