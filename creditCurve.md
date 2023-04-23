
### CDS Index Curve Adjustment


The methodology of credit default swap index (CDSI) curve adjustment serves the purpose of making adjustment to the credit spread curve of each reference name in the index portfolio such that the market price of the index can be reproduced using these constituent curves. The adjusted index constituent curves are then used to price the standard collateral debt obligation (CDO) tranches based on the index portfolio.

Within the credit derivative modelling framework, the valuation of CDS index, by employing index constituent curves, has been previously approved for the CDSI option valuation model and found consistent with the method proposed by Bear Sterns and Morgan Stanley.  The adjustment procedure involves iteration by multiplying all the constituent credit spread curves with a scaling factor. 


The purpose of the model is to make adjustment to the credit spread curve of each reference name in the credit default swap (CDS) index portfolio such that the market price of the index can be reproduced using these individual curves. The adjusted index constituent curves are then used to price the standard collateral debt obligation (CDO) tranches based on the index portfolio, which is essential to build a base correlation curve.

Market quoted CDS indices, such as CDX or Tracer-X, are defined as the fair premium paid over a stream of risky coupons in exchange of default protection on standardized portfolios. Unlike a stock index it is not simply the weighted average of credit spreads for the reference names in the portfolio.  A CDS index on a portfolio can be viewed as the b/e spread to an untranched basket credit default swap on that portfolio. As a result, an index position at a level   is equivalent to a portfolio of CDS on the reference names, where all CDSs are entered at the same spread  . Individually, each CDS does not trade at b/e spread, but the portfolio as a whole does. Furthermore, market quoted index assumes a flat credit spread curve and 0.40 recovery rate.
 
Within the credit derivative modelling framework, pricing an index by employing constituent curves of the index portfolio has been previously approved and found consistent with the one proposed by Bear Sterns and Morgan Stanley.  

For some reasons, such as quoting convention differences and liquidity, a direct pricing from constituent curves won’t be the same as the market quoted index implied price. An adjustment is needed. The proposed method involves the following steps:


References:

[zenodo pdf](https://zenodo.org/record/7373680/files/creditCurveAdjustment.pdf)

[bitbucket cppi](https://bitbucket.org/timxiao1203/profit-and-loss-explanation/downloads/PnLExplain.pdf)

[github cms](https://github.com/cfrm17/ConstantMaturitySwap)

[github lgm](https://github.com/cfrm17/lgmCalibration)

[github interpolation](https://github.com/cfrm17/quadraticInterpolation)
