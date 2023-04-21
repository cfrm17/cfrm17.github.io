
### Credit Derivative Pricing 


We propose default correlation model and four credit default derivative pricing models, namely, single name credit default swaps with counterparty risk, First-to-Default basket default swaps, FirstNofN basket default swaps, and FirstLoss trades. 

The purpose of the default correlation model is to predict the probabilities of single- and multiple- default events for a collateral asset pool, which are then converted into pricing for various credit derivatives. The model is built upon the hazard rate curves with certain assumptions on default correlation among the obligors in the collateral pool. The hazard rate curve, which represents the unconditional default probability of an obligor, is calibrated by the market information of single name credit default swap and has been re-reviewed in phase one

The normal copula function is a multivariate cumulative normal distribution with correlation matrix  . Applying the normal copula function to the modeling of correlated default events of a collateral asset pool, the uniform random variables are mapped to the default probabilities with standard normal distribution. The normal copula function, or the cumulative joint default probability for the collateral pool with n assets, can be expressed as

With the joint distribution described by the multivariate normal distribution, the correlated default times can be calculated by either closed form solution or by Monte Carlo simulation. The details of the copula model can be found in the cited papers.

The credit derivatives can be treated in a two-leg fashion: fee leg and protection leg. The protection buyer of the pays a fee to the seller periodically of the protection in exchange for a contingent payment in the event that the reference obligor(s) default before the maturity of the trade. If the reference entity is a collateral pool, the default events of the obligors are correlated and should be modelled by default correlation model.

The CDS with counterparty risk is a credit derivative in which we could recovery certain fraction of the forward contract value, if the counterparty defaults before the reference obligor.  



References:

[zenodo pdf](https://zenodo.org/record/7832032/files/CreditDerivativePricing.pdf)

[archive bond](https://ia904700.us.archive.org/14/items/bondAmericanOption/bondAmericanOption.pdf)

[gitbook inflation](https://finwhite.gitbook.io/inflationcap/)

[github reverse](https://github.com/cfrm17/reverseConvertibleModel)

[github collateral](https://osf.io/zuhcw/download)
