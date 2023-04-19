
### Local Vol Greek 

Calculation of the Greeks in the local volatility model is difficult because recalibrating the local volatility surface tends to result in high numerical error terms. While this appears to be OK for first order Greeks, for higher order Greeks we are forced to make some approximations. Here is the full list of Greeks.

Delta – calculated by perturbing spot up and down by 0.1%, re-calibrating forwards and local vols, and using central finite difference approximation

Vega – calculated by perturbing volatility up and down, recalibrating local volatility surface, and using central finite difference approximation

SkewVega – calculated by perturbing skew, recalibrating local volatility surface, and using finite difference approximation

HedgeRho – calculated by bumping the yield curve (ref. https://finpricing.com/lib/IrCurveIntroduction.html) used for forwarding, recalculating the forwards but not recalibrating the local volatility surface. As such this is an approximation, which assumes that dLocalVol/dHedgeRho is small

DiscountRho – calculated immediately when the payoff has a single known payment date. Otherwise calculated by bumping the curve and recalculating the discount factors within the grid. Note that the local volatility surface is unaffected by the discount rho and does not require calibration.

Gamma – Unfortunately gamma calculated by finite difference with recalibration off the volatility surface is not sufficiently stable. We therefore use an approximation. First note that 


References:

[archive pdf](https://ia904700.us.archive.org/33/items/local-vol-greek/LocalVolGreek.pdf)

[gitbook gic](https://finwhite.gitbook.io/gicgreek/)

[github arrear](https://github.com/timxiao1203/ArrearQuantoCMS)

[core irc pdf](https://core.ac.uk/download/334593149.pdf)

[core irc](https://core.ac.uk/works/8882346)

