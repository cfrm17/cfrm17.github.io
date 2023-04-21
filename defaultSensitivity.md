
### Default Sensitivity


The default sensitivity test in Scenario Manager is implemented by setting the default time of the perturbed obligor to be the valuation date when the present value of each tranche is calculated, no matter when that obligor defaults in the generated Monte Carlo scenarios. Compared with other models, the implementation of Scenario Manager model is simple, direct, and efficient. However, the joint default events generated in the MC scenarios remain unchanged, which is an approximation of the realistic situation.

Through testing we have found that this approximation is good when the correlation is weak. In general the Scenario Manager model can be viewed as an intermediate one between the models with 30,000 bps credit spread shock to the perturbed obligor and the model with no correlation between the perturbed obligor and the other obligors in the portfolio.  

The Risk Engine has two functions: default sensitivity test and credit spread sensitivity test. It is implemented by the Scenario Manager, an autorun program, which manages the calculation of MTM value of the deal and the sensitivity Greeks. 

Default sensitivity test is a kind of stress tests matching the situation that a credit default event of an obligor has occurred or is perceived to be imminent. It is implemented by finding the change of Present Value (PV) for the tranches when the default time of an obligor is perturbed. The Scenario Manager Model is implemented by setting the default time of each obligor to be the valuation date when calculating the present value of each tranche, no matter when that obligor defaults in the generated Monte Carlo (MC) scenarios. 

In this measure both the default times of the perturbed obligor seen by other obligors in the portfolio and the default correlations between the perturbed obligor and other obligors remain unchanged. This is not realistic because the MC paths of all the other obligors are generated without the updated information that the perturbed obligor has defaulted. We only perturbed the primitive default time of the perturbed obligor to be the valuation date while the joint default events incurred by this perturbed obligor is not re-simulated accordingly.    

In order to test the Scenario Manager model, three other measures of default sensitivity which sound reasonable are considered:


References:

[zenodo pdf](https://zenodo.org/record/7373904/files/DefaultSensitivity.pdf)

[archive gic](https://ia601507.us.archive.org/23/items/gicPricing/gicPricing.pdf)

[github swap](https://github.com/cfrm17/equityForFloatSwap)

[core spread pdf](https://core.ac.uk/download/534866631.pdf)

[core spread](https://core.ac.uk/works/127929800)

