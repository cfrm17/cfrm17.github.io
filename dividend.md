
### Dividend Risk


OSFI recommended that dividend risk should be captured in market risk framework. To achieve that, a dividend risk model is developed by Market Risk (MR) and will be implemented in system. The model calls for the introduction of new dividend risk factors as the expected dividend amount of an equity asset, either a stock, or a basket of stocks, or an equity index. 

This new risk factor can be regarded as a “companion” to the spot price equity risk factor currently in system in the sense that for each underlying equity asset, regardless of types, there is a spot price risk factor and also a dividend risk factor, even for those that market does not expect to pay dividend. Under the proposed model and methodology, the position sensitivity and simulated scenario will be both zero if the underlying asset is not expected to pay dividend so that no dividend risk is artificially produced. 

Currently, we generate 10,000 scenarios of non-dimensional relative return of equity market risk factors, a total of 160 equity implied volatility risk factors and 113 index price risk factors, among about 5000 global market risk factors, in simulation 1. Sensitivity feed is used to map risk factors, assign Greeks to risk factors, and create equity price risk factors if necessary. 

Simulation of price risk factors is done in Simulation 3 based on scenarios from Simulation 1. Simulation of derived price risk factors, primarily for baskets and indices, is done in Simulation 4 based on scenarios from Simulation 3.  New risk factors are created if mapping does not find a match and default equity index market risk factor, beta and idiosyncratic volatility are assigned so that the scenario for this risk factor can be simulated. In the case of implied volatility risk factor, mapping will simply assign default risk factor rather than creating new risk factor.

There are currently about 4500 equity names from monthly calibrated beta files, in which beta and idiosyncratic volatility for each name on its respective indices, selected from the 113 equity price indices in market risk factors, are given.  In addition, there are about 2000 equity names not mapped to the equity names on the above beta file, as well as about 500 equity basket or index names, to be created each day. All these equity names, total about 6500, either on beta file or created daily, will be simulated in Simulation 3. The basket or index names are considered derived risk factors to be simulated in Simulation 4. Note that we assign three risk factors to each equity name or basket/index name for risk decomposition purpose: the three risk factors are to account for total risk (risk type: TOT), market risk (MKT), and equity specific risk (SPF). 

Under the proposal, there will be a newly introduced dividend risk factor for each equity name or basket/index name. Hence, the total number of new risk factors is less than about 7000, considering that the basket and index names are no longer considered derived risk factor for dividend purpose, and thus there is a reduction in equity names as components of some basket or index. 


References:

[Hcommons double](https://works.hcommons.org/records/z2m18-px347/files/doublewindowdoublebarrieroption.pdf?download=1)

[github power](https://github.com/cfrm17/PowerSwap)

[github tunnel](https://github.com/cfrm17/RatioTunnelOption-)

[github asian fwd](https://github.com/cfrm17/ReciprocalAverageRateForward)
