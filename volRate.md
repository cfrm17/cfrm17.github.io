
### Volatility Closing Rate 


We use the Omega type models to model the implied volatility skew for commodity derivatives.  These surfaces are incorporate moneyness and time to maturity into the skew definition and are a function of calibrated parameters (skew, wing, boost etc).

To populate the closing rate for implied volatility skew risk factors, it will be necessary to implement the forward-delta based Omega skew models and use the Brent root finding algorithm to solve for the closing rate.  This function spec will outline this procedure.

The vega allocation is outlined in the MRA functional spec on the skew introduction into system.  Here we briefly review the methodology and then go through an example of vega allocation.

One way to think of the u and the v above, are as the weights used in linear interpolation.  We now look at the vega allocation for a specific deal, 25878, an Asian call option on NYM_WTI.  Here is relevant information for the deal specific to vega allocation:


References:

[Zenodo Greeks](https://zenodo.org/records/14996548)

[github fader](https://github.com/cfrm17/FadeOption)

[github delta](https://github.com/cfrm17/FxOptionDelta)

[github asian](https://github.com/cfrm17/FxAsianFuturesOption)
