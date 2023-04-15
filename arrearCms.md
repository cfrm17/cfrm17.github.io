
### Arrear Quanto CMS Analytics

An arrear quanto constant-maturity-swap (CMS) is a swap that pays coupons in a different currency from the notional and in arrears. The underlying swap rate is computed from a forward starting CMS.

Assumes that, under the coupon payment currency (SEK) risk-neutral probability measure, the forward swap rate process corresponding to each swap rate fixing follows Geometric Brownian motion with drift.  Each forward swap rate process is then convexity adjusted, and is furthermore expressed under the notional currency (FRF) risk neutral-probability measure by means of a quanto adjustment.

We assume that, under the SEK risk-neutral probability measure, the forward swap rate process follows Geometric Brownian motion with drift. The initial forward swap rate is calculated, and is then convexity adjusted.

Here the convexity adjustment is from a par bond specified by • three year maturity, • annual coupon, set equal to the initial forward swap rate, • yield-to-maturity equal to the coupon rate.

The initial forward swap rate is also quanto adjusted. We note that the correlation used in the spreadsheet is between the FRF to SEK exchange rate and the SEK swap rate.

Finally the respective quanto and convexity adjusted initial forward swap rates are added together to produce the initial forward swap rate under the FRF risk-neutral probability measure.

We note that the common currency unit in Europe is now taken to be the EURO. Furthermore, the exchange rate from the EURO to an associated currency (e.g., FRF) is fixed, so there is no foreign exchange risk. Therefore FP London uses a common curve, EURIBOR, for discounting; that is, is replaced by the equivalent discount factor from the EURIBOR curve.

References:

[pdf](https://osf.io/g6tp5/download)

[Zenodo futures swaption pdf](https://zenodo.org/record/7308915/files/CommodityFutureSwaption.pdf)

[Zenodo futures swaption](https://zenodo.org/record/7308915)

[Zenodo faderin pdf](https://zenodo.org/record/7313954/files/FaderIn.pdf)

[Zenodo faderin](https://zenodo.org/record/7313954)



