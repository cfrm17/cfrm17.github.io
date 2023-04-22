
### Credit Contingent Interest Rate Swap 


A credit contingent interest rate swap is an option that grants its holder the right, but not the obligation, to enter into an interest rate swap (IRS) at the time when its reference obligor defaults. The premium to be paid on the underlying IRS is fixed in advance at some strike level. The notional amount of the swap is a function of a predetermined fixed amount and the recovery rate of the reference obligor. The model can also be employed to back out an implied correlation between the interest rate and the default arrival of an obligor.

The valuation model is a simplified closed form solution, in which a lognormal process for the swap rate and an Ornstein-Uhlenbeck (OU) process for the hazard rate are assumed.  Both processes are one-factor models and they couple to each other in a standard way. The volatility skews and smiles for swap rates are calculated via a stochastic volatility model, namely SABR model. The default probability of the reference obligor is calibrated to the credit default swap (CDS) market and the volatility of the hazard rate is implied by the market information of CDS options (CDSO).  

The correlation between the swap rate and the hazard rate of an obligor is not a market observable and should be implied from the CCIRS market. For an obligor whose market implied correlation information can not be found, a historical analysis has to be used to obtain a reasonable estimate and a pertinent reserve has to be set up. A reserve methodology has been proposed by GRMMR London to address parameter uncertainties and approximations in the model. 

The credit contingent interest rate swap (CCIRS or CCDS) valuation model serves the purpose of pricing an option that grants its holder the right, but not the obligation, to enter into an interest rate swap (IRS) at the time when its reference obligor defaults. The premium to be paid on the underlying IRS is fixed in advance at some strike level. The notional amount of the swap is dependent on a predetermined fixed amount and the recovery rate of the reference obligor.  

In essence, a CCIRS trade can be regarded as an interest rate swaption with two special features. One is that the maturity of the swaption is the default time of the reference obligor, which is unknown. The other feature is that, although the strike of the underlying swap is predetermined, the tenor and the notional amount of the underlying swap are dependent on the default time and recovery rate of the reference obligor, respectively. The trade provides a hedging of the counterparty risk in an IRS. 


References:

[zenodo pdf](https://zenodo.org/record/7362947/files/ccds.pdf)

[archive warrant](https://ia903404.us.archive.org/22/items/eq-warrant-8/EqWarrant-archive.pdf)

[gitbook payment](https://finwhite.gitbook.io/paymentneuralnet/)

[github asian](https://github.com/cfrm17/callableAsian)

[github coupon](https://osf.io/x2rf8/download)
