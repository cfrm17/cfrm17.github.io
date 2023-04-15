
### Extendable Swap Valuation

An extendable swap represents a forward swap agreement with an option of extending the swap for another term (swaption). Other irregular swaps include accumulator swap (see https://finpricing.com/lib/FxAccumulator.html)

The valuation model assumes the swap rates for different terms to be correlated log-normally distributed random variables and uses the Haselgrove integration method for pricing the deal. 

We use analytical formulas for forward swap and swaption valuation: the swap price is calculated as the difference between a bond par and the bond’s price, and the swaption price is evaluated from the Black’s formula.

The model estimates the swap price as a risk-neutral expectation of the difference between the bond price whose yield-to-maturity is the swap rate and the bond’s par. The swap rate is considered a log-normally distributed random variable. 

The forward swap rate is adjusted to convexity is taken as the mean of the swap rate’s distribution. The price of the swaption is estimated by using Black’s formula. The off-diagonal term of the correlation matrix of the swap rates was estimated from historical data. 

To provide the ability of controlling interest and swap rates for our testing, the CAD_BA curve was constructed as a flat yield curve at a prescribed yield level (of 5% or 25%). The swap rates were set to those retrieved from the CAD_BA curve for the first year of the deal, and therefore they were supposed to turn the swap price to zero.

Relating the test values to the notional amount may not be the right measure in every case. If the absolute prices are important, the users should exercise caution in the cases of volatilities exceeding 50% combined with time lag between the deal and start date longer than 3 years or in the cases of interest rates exceeding 15%.

The model estimates the swap price as a risk-neutral expectation of the difference between the bond price whose yield-to-maturity is the swap rate and the bond’s par. The swap rate is considered a log-normally distributed random variable.

The forward swap rate is adjusted to convexity is taken as the mean of the swap rate’s distribution. The price of the swaption is estimated by using Black’s formula. The off-diagonal term of the correlation matrix of the swap rates was estimated from historical data.



References:

[osf pdf](https://osf.io/23w9h/download)

[zenodo cds curve](https://zenodo.org/record/7373116/files/CDSHCurve.pdf)

[zenodo cds curve](https://zenodo.org/record/7373116)

[Zenodo CDSO pdf](https://zenodo.org/record/7373465/files/CDSO.pdf)

[Zenodo CDSO pdf](https://zenodo.org/record/7373465)

[researchgate](https://www.researchgate.net/profile/Tim-Xiao/publication/337496817_The_Valuation_of_Interest_Rate_Swap_with_Bilateral_Counterparty_Risk/links/6427499066f8522c38e94f11/The-Valuation-of-Interest-Rate-Swap-with-Bilateral-Counterparty-Risk.pdf)



