
### FX Spot Rate Calibration


In principle, one should be able to calibrate rho from the market data, for example,  by applying maximum likelihood, or least squares, or other estimation technique to the historically realized sequence. However, given the time dependence of the long run mean in our model, these methods may be challenging to implement. As an alternative we may proxy local volatility with either the historical or the implied volatility, as it is done for the current production model.

For this latter approach, a natural first choice is to consider the statistics of the historical spot FX rates. For example, one could estimate the annualized standard deviation (SD) of log return series, taken over a sampling window of adequate length – long enough to smooth-out the high frequency (daily, weekly) variation in the FX rates, but short enough to allow for the ongoing market conditions to manifest themselves in a timely manner. However, using historic FX time series has the drawback that regardless of the smoothing procedure, the volatility is “backward looking”, and representative of past behavior, which may not be desirable for the simulation of future rates.

The alternative choice is to use the FX implied volatility of the (at-the-money) FX options. Compared to the use of historic volatility, the FX IV is a “forward looking” measure of the variability of the FX log return (backed out from the Black-Scholes pricing formula), reflecting the market consensus of future behavior of the spot FX rates, as is based on the currently available information to the market participants. FX IV data are readily available for both testing and production purposes, covering various maturities and expiry terms up to 5-years, with history going back 10 years or more on select currencies. 

One is then left with the task of selecting a representative term to expiry and of a smoothing procedure, to mute the impact of high frequency changes in FX IV series.

The rationale for this calibration choice is that the Model User requires a bounded envelope for the simulated rates that is in agreement with the envelope of the historically realized FX spot rates. The simplest approach is to impose the equality of the theoretical envelope of the simulated rates at a certain long term bucket (say, 15-years, which corresponds to about two business cycles) with the historically realized envelope of the FX rate time series. The choice of the interquantile range (5% - 95%) is dictated by the ubiquity of this range in exposure estimation and, to a certain extent, by the length of available history for FX spot rates.  

References:

[Guaranteed note](https://www.researchgate.net/publication/385743880_Pricing_Guaranteed_Withdrawal_Notes)

[Guaranteed note pdf](https://www.researchgate.net/profile/Tim-Xiao/publication/385743880_Pricing_Guaranteed_Withdrawal_Notes/links/6733981a69c07a4114454fdf/Pricing-Guaranteed-Withdrawal-Notes.pdf)







