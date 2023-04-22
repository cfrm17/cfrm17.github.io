
### Forward Starting CDO  



The forward starting CDO (FSCDO) valuation model serves the purpose of pricing a forward starting CDO (FSCDO) tranche. An FSCDO trade is defined as an agreement to enter into a CDO trade at some time in the future. Unlike a usual forward starting instrument in the interest rate world, the obligors in the collateral pool of the FSCDO may default before the forward starting date, which makes the pricing of such trades complicated. Furthermore, the FSCDO involves the forward start date and the trade maturity; hence a pertinent valuation model needs to be calibrated to the market implied correlation information with a full term structure.

In the past three years the structured credit derivative modeling has witnessed the emergence of the vanilla CDO trades pricing using market implied correlation information, and the standardization of the normal copula model within the base correlation framework.  

The occurrence of the more complicated structure, such as the FSCDO trade discussed in this report, leads to alternative ways of explaining the correlation information implied by the market standard iTraxx and CDX indices.  In the initial modeling approach, a copula is normally assumed first, for example normal copula, t copula, etc. The random factor loading approach relaxes this assumption to some extent by assuming the factor as a function of the latent variable hence the joint marginal distribution is no longer normal. The latest development moves even further. 

As proposed by several authors, a non-parametric modeling framework is employed to match the market information. For example, in the perfect copula model, the assumption of any copula form is dropped, and the copula function itself is implied by the market information. In the Gaussian mixture model, three correlation values and their corresponding weights are found to match five market quotations of an iTraxx or CDX index.

The FSCDO model belongs to the non-parametric category.  In order to price the FSCDO with the market implied information of different terms, the model employs a WMC method. The following procedures are involves:

By using the normal copula MC simulation model, the prior correlated default scenarios of the obligor in the collateral pool are simulated with a set of correlation parameters. Currently we choose five correlation values 0, 0.2, 0.4, 0.6, and 0.95, with the minimum number of simulation associated with each correlation being 100,000.  The correlated default times of obligors in each MC scenario are recorded. 


References:

[zenodo pdf](https://zenodo.org/record/7374358/files/FSCDO.pdf)

[archive inverse](https://ia904704.us.archive.org/2/items/callableInverseSwap/callableInverseSwap.pdf)

[gitbook partial](https://finwhite.gitbook.io/partialswap/)

[github futures](https://github.com/cfrm17/equityFutures)

[osf market](https://osf.io/rbxqz/download)
