
### All-In Gamma Shocks

In the Commodity framework, risk factors for NG pipelines are currently defined with respect to base and spread (over NYM_NG).  The delta sensitivities in RDR are given for the base and spread, but the gamma is an “all-in”, meaning it calculated with respect to base plus spread curve.  Because we do not have separate risk factors for the all-in curves, we modify shocks generated for the base and spread curves to construct those for the all-in curves.  

We can see that the shocks to the all-in curve require the relative and absolute changes of the base curve and spread respectively, as well as the closing rate of base curve.

In the framework, the shocks from the defined risk factors are mapped back to the market instruments.  For instance, a typical deal might have the following delta and gamma and sensitivities:

The all-in gamma sensitivities from RDR have a label which is distinctive and can also all easy mapping to the associated spread.  The “NG” curve will always be the base curve.

Given the base and spread scenarios, those for the all-in curve can be generated and should be mapped according to spread name and contract date.  For instance, in the example above the AECOM: 201404 AllIn point would take absolute change from the AECOM: 201404 contract, and the base relative change and closing-rate from the NG: 201404


References:

[Hcommons barrier](https://works.hcommons.org/records/9kywg-b2d48/files/barrierprobabilitynew.pdf)

[github reciprocal](https://github.com/cfrm17/FxReciprocal)

[github variance](https://github.com/cfrm17/fxVarianceSwap)

[github capped](https://github.com/cfrm17/cappedAccumulator)
