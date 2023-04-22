
### Hazard Rate Curve 



The hazard rate curve defines the default probability of an obligor, serving as one of the fundamental components of all credit derivatives models.  Within the current GSP credit derivatives modelling framework, the hazard rate curve is calibrated using the market information of the credit default swap (CDS).  

By definition the hazard rate has to be positive to ensure a larger than zero default probability within any period of time. It is a function of credit spread curve, recovery rate, and interest rate.  The credit spread curve is defined as a set of the market quoted CDS spreads with different terms to maturity. We assume one constant recovery rate for each obligor. Normally we assume 0.35 or 0.4 for most of the obligor and 0.15 for subordinate names. 

Given all the input parameters, the hazard rate curve is calculated via bootstrapping. There exists a possibility of failing to building a valid one, either because 1) the input implies a negative hazard rate or 2) a value outside of root finding range. In the GSP model, a root finding scheme is used in which we set the searching range to be 0 and 20.  

Note that this range is very large and a hazard rate 20 implies that the average default time would be within a month. From the viewpoint of modelling, this assumes almost an instant default of the underlying obligor and there is no need to build a hazard rate curve.  However, technically this restriction puts an upper limit on the valid credit spread that the model can handle. As analyzed in the next section, with the conventional recovery rate assumption we set this limit be 100, 000bps. 

The recovery rate can not be exactly one for any non-zero credit spread level. Because Eq.(6) can not be solved explicitly to check if the hazard rate is larger 20, we use an approximation to estimate the maximum recovery rate. If we assume a flat credit spread curve and ignore the discount factor, the hazard rate curve reads:


References:

[zenodo pdf](https://zenodo.org/record/7373116/files/CDSHCurve.pdf)

[archive callable](https://ia803403.us.archive.org/32/items/eq-callable-15/EqCallable-archive.pdf)

[gitbook mbs](https://finwhite.gitbook.io/mbs-liquidation-model/)

[github cds](https://github.com/cfrm17/CdsTermStructure)

[github asian](https://osf.io/e9wb3/download)
