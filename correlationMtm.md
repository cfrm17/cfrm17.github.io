
### Correlation MTM 




The model for valuation of CDOs is well documented. An essential input into the model is the correlation between the obligors in the collateral pool. Historically, this correlation has been derived using a KMV based approach.

In an attempt to make the valuation of these trades more consistent with market conditions, a new method for implying these correlations from the tracer market has been proposed. The methodology involves two steps: implying a correlation from the tracer market and then mapping the actual trades to these tranches to determine the implied correlation used to value these.

Specifically, we examined the proposed procedure for mapping tracer tranches to non-index CDO tranches in a portfolio. The goal of the procedure is to be able to use the tracer market to imply a correlation suitable for marking the market of the CDOs.

We first need to determine an market implied correlation for the tracer tranches. In order to do so, each tranche is valued at various constant correlations ranging from 0 to 0.7 in increments of 0.1. The implied correlation for each tranche is then found by linear interpolation by matching the model price with the market price. Note that this approximation might not be ideal if the market value versus correlation is not linear.

The figure 1 shows the various values for the tracer tranches using the model under various (flat) correlations. Note that there are two potential sources of difficulty or error that may arise in implying a correlation:

The values are not linear versus correlations, especially for the mezzanine tranches. Therefore a non-linearity error will occur with varying degrees of materiality depending on where the market is trading. Note that this error is purely a function of efficiency, as this could be reduced with increased granularity 



References:

[zenodo pdf](https://zenodo.org/record/7378011/files/CorrelationMtm.pdf)

[archive gic](https://ia601508.us.archive.org/28/items/flexibleGic/flexibleGic.pdf)

[gitbook cms](https://finwhite.gitbook.io/cmsconvexity/)

[github binary](https://github.com/cfrm17/binaryReturn)

[osf var](https://osf.io/m9j7v/download)
