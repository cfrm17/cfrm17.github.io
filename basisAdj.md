
### CDS Index Basis Adjustment


The model serves the purpose of computing basis adjustments for credit spread curves of the constituent obligors of the indexes such that the market price of the index can be repriced exactly. These adjusted index constituent curves are then used to compute index base correlations and mapped base correlations for bespoke trades, price the standard index CDO tranches, and calculate risks for constituent obligors.  

In the submitted model, the basis adjustment is calculated by applying one stepwise constant term structure of scaling factors to all individual hazard rate curves. The market standard models are employed in the valuation of MTM of the quoted index via the constituent curves and quoted index premiums. The term structure of the scaling factor is computed through bootstrapping such that the MTMs of the indexes of all terms can be repriced.

The implementation of the submitted model was first verified by testing against an independently developed test model. The implications of underlying assumptions in the model were tested against several benchmark models. The internal error tolerance control in the bootstrapping and the choice of the flat term nodes of the indexes were assessed and found appropriate as well.

It is important to note that, from the viewpoint of mathematical modeling, there are many ways to make such adjustments and the methodology of adjustment is only one of the choices. Each choice bears different assumptions on the embedded index basis risk and, to our best knowledge to date, there is no generally accepted market convention of making such adjustment. The test results indicate that, as far as the calibration of the base correlation and the valuation of an index CDO trade are concerned, the differences among those choices are immaterial. It is also indicated that the differences mainly resides in the term nodes that are far from the index maturities, which may be material depending on the hedging strategy for index CDO trades.

The purpose of the submitted model is to make adjustment to the credit spread curve of each reference name in the credit default swap (CDS) index portfolio such that the market price of the index can be repriced using these individual curves [1]. The adjusted index constituent curves are then used to calculate index base correlations and mapped base correlations for bespoke CDO trades, price the standard CDO tranches, and calculate risks for constituent obligors.  

Market quoted CDS indices, such as CDX or iTraxx, are defined as the fair premium paid over a stream of risky coupons in exchange of default protection on standardized portfolios. Unlike a stock index it is not simply the weighted average of credit spreads for the reference names in the portfolio. An index has a fixed coupon and is traded by price. It the market convention that this price can be converted to quoted spread   with a flat curve and 40% recovery rate assumptions. As a result, an index position at a quoted spread level   is equivalent to a portfolio of CDS on the reference names, where all CDSs are entered at the same spread . Individually, each CDS does not trade at spread , but the portfolio as a whole does. Furthermore, market quoted index assumes a flat credit spread curve and a recovery rate 0.4.
 
On the other hand, single name credit default swaps for the index constituent obligors have become very liquid. Although trading an index and a portfolio single name CDS of its constituent obligor are essentially equivalent, a basis can be observed between the market quoted spread and the index spread calculated using constituent curves.  Therefore an adjustment is needed in order to use the constituent credit spread curves to price the standard index CDO tranches for the purpose of computing marking-to-market (MTM), risks, base correlation curves, and loss ratios.



References:

[zenodo pdf](https://zenodo.org/record/7387930/files/basisAdjustment.pdf)

[archive ratchet](https://ia601506.us.archive.org/33/items/ratchetSwap/ratchetSwap.pdf)

[gitbook credit](https://finwhite.gitbook.io/creditriskcalculator/)

[github basket](https://github.com/cfrm17/basketAsianRpo)

[github quanto](https://osf.io/2qjps/download)
