
### Risk Measures for Index Tranches 


The purpose of the model is to calculate the credit spread sensitivity, correlation sensitivity, and default sensitivity via analytic methods for index CDO trades and bespoke CDO trades. 

The credit spread sensitivity is defined as the change in the MTM by perturbing the credit spread by a small amount; the default sensitivity is calculated by assuming that one obligor in the collateral pool defaults right away; and the correlation sensitivity is computed by perturbing the index base correlations by a small amount. 

The new components developed in the Oscar/Fritz credit library enable us to capture risk more accurately. Previously, the index basis adjustment, base correlation calibration, and CDO2&3 trade equivalent CDO re-flattening (RE-CDO) were implemented outside the Oscar/Fritz library and there was no way to make corresponding adjustments in perturbed scenarios. In the new model, we can recalculate the basis adjustments, remap base correlations, and re-flatten RE-CDOs in the perturbed scenario. 

The credit spread sensitivity is switched to a bucketed one (CSPDH). In the model, parallel shift credit spread sensitivity has been used for many years. However, recent development in the market, especially the popularity of longer term trades, makes this measure inaccurate.
 
A new method to compute credit spread and correlation sensitivities are adopted in the submitted model. As outlined in the Section 1, those sensitivities are calculated by separating all relevant risk factors in the form of Jacobians and then combining them together, instead of a full bump and revaluation approach.

The advantage of the analytic sensitivity model is the computational efficiency, which allows us to compute the sensitivities by taking into account of all relevant risk factors. For example, it would be too time consuming to do a full bump and revaluation approach for a CDO2&3 trade. 

In the analytic sensitivity model, the internal shock amount is set to be  on a term node. Considering the fact that a CDO may have more than a hundred obligors, this shock amount is so tiny that, from the viewpoint of mathematical modeling, it is a “purer” delta than what we normally think of. When we use this more or less “theoretical” limit delta for any practical purpose, where a larger finite change in credit spread is encountered, we should pay more attention to any possible gamma effect. Normally this can be checked by a full bump/revaluation approach. 



References:

[zenodo pdf](https://zenodo.org/record/7388002/files/RiskMeasuresIndexBespoke.pdf)

[archive libor](https://ia601500.us.archive.org/4/items/liborSwapModel/liborSwapModel.pdf)

[gitbook mbs](https://finwhite.gitbook.io/variableratembsvaluation/)

[github bond](https://github.com/cfrm17/bondOption)

[osf spread](https://osf.io/4kcrh/download)
