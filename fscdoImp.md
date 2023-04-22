
### Forward Starting CDO Model Implementation


The forward starting CDO (FSCDO) valuation model serves the purpose of pricing FSCDO trades, which are defined as a forward agreement to enter into a CDO trade at some time in the future. Any obligor defaults before the forward starting date will be replaced by a risk free asset with the same notional amount.

A non-parametric approach is adopted in the model. A Monte Carlo (MC) simulation is first employed to generate a large number of prior correlated default scenarios with a set of different correlation assumptions. The weight of each MC scenario is computed by the weighted Monte Carlo (WMC) method, such that the credit spreads of each obligor and the market implied spot tranche values with different terms can be repriced. Then the MC scenarios associated with the calibrated weights can be used to price the FSCDO trade.

To our best knowledge to date, there is no directly observable market information on the FSCDO. The methodology of the model is considered acceptable, based on the fact that the model can be calibrated to the pertinent spot market information with different terms, effectively deal with market implied correlation skew structure, and reasonably model the default events before the forward starting date. However, there are two embedded model uncertainties. One is the calibration process of WMC in which the optimization of hundreds of instruments is involved for a normal FSCDO trade. This task is difficult and it is unlikely to achieve a perfect calibration to all instruments. The selection of the spot calibrating instruments, specially the spot tranches, also contributes to the uncertainties of the calibration.  The other uncertainty resides in the generation of the prior MC scenario. Two different choices would give different prices of the forward trade, even if both can be successfully calibrated to the spot market information. 

As an effective way of managing the model uncertainties, a model risk reserve is set up by benchmarking against the most conservative parameter scenarios. At the present time those scenarios are found through an extensive testing on a trade by trade basis. When we start to accumulate positions in FSCDOs, well defined conservative scenarios will be justified and established.

In the model setup, the results of the optimization can be tracked in two ways. First a log file can be generated with the example given in Figures 1(a) and 1(b). In Fig. 1(a), a successful calibration is achieved while in Fig. 1(b) the calibration fails. In the latter example, the optimization stops because objective function exceeds limits (100) and shows no sign of convergence. Second, a message is shown to imply in the pricing spreadsheet that how many iterations are performed before the convergence is reached. If this number reaches the maximum,  it indicates that most likely no convergence is reached. The calibration results of the spot tranche values are exported to show how good the calibration of those tranche values. However,  we should be cautious to take these results the criterions as the calibration, because the largest portion of calibration instruments are acutally the credit spreads of each obligor. The calibration results of those credit spreads are not exported in the model. Normally the calibration of a credit spread for an obligor can be manually verified by setting the notional amount of all other oblgors to zero. 


References:

[zenodo pdf](https://zenodo.org/record/7374369/files/FSCDOImplementation.pdf)

[archive reverse](https://ia803407.us.archive.org/2/items/eq-reverse-18/EqReverse-archive.pdf)

[gitbook seller](https://finwhite.gitbook.io/sellerswap/)

[github hazard](https://github.com/cfrm17/hazardRateCalibration)

[github inflation](https://github.com/timxiao1203/InflationSwap)
