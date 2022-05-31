
### Counterparty Credit Risk Simulation Methodology

Counterparty credit risk (CCR) is the risk of loss that will be incurred in the event of default by a counterparty. It will be incurred in the event of 
default by a counterparty. Only over-the-counter (OTC) derivatives and financial security transactions (e.g., repo) are subject to counterparty risk. 
If one party of a contract defaults, the non-defaulting party will find a similar contract with another counterparty in the market to replace the 
default one. That is why counterparty credit risk sometimes is referred as replacement risk. The replacement risk is the MTM value of a counterparty 
portfolio at the time of the counterparty default.

Counterparty credit risk measure is credit exposure. As credit exposures in future are stochastic, one needs to simulate market evolution in order 
to quantify CCR. This presentation provides some details about CCR simulation.

Counterparty credit risk refers to the risk that a counterparty to a bilateral financial derivative contract may fail to fulfill its contractual obligation 
causing financial loss to the non-defaulting party. The risk that a counterparty defaults prior to expiration of a contract. If one party of a contract 
defaults, the non-defaulting party will find a similar contract with another counterparty in the market to replace the default one. That is why 
counterparty credit risk sometimes is referred as replacement risk. The replacement risk is the MTM value of a counterparty portfolio at the time of the 
counterparty default. Credit exposure (CE) is the cost of replacing or hedging a contract at the time of default. Credit exposure is uncertain (stochastic) 
so that Monte Carlo simulation is needed

To calculate credit exposure or replacement cost in future times, one needs to simulate market evolutions. Simulation must be conducted under the 
real-world measure. One could use a simple but inaccurate solution, or accurate but complex approach. Some vendors and institutions use this simplified 
approach. Only a couple of stochastic processes are used to simulate all market risk factors. They use Vasicek model for all mean reverting factors
dr=k(θ-r)dt+σdW where r – risk factor; k – drift; θ – mean reverse; σ – volatility; W – Wiener process. And use Geometric Brownian Motion (GBM) for all 
non-mean reverting risk factors: dS=μSdt+σSdW. The calibration results for different risk factors are different from each other.

Simulate yield curve or zero curve represented by yield rates or zero rates rather than swap curve represented by futures and swap rates. There are many 
points in a yield curve, e.g., 1d, 1w, 2w 1m, etc. One can use Principal Component Analysis (PCA) to convert, say, 20 points into 3 point drivers. 
Using PCA, you only need to simulate 3 drivers for each curve. But please remember you need to convert 3 drivers back to 20-point curve at each path 
and each time step.



Reference: 

[CCR Simulation](/ccrSimulation-2.pdf)

[FlipHtml5 ccr simulation](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamkDN4UzM5ITPkl0av9mY)

[Hcommons ccr simulation](https://hcommons.org/deposits/download/hc:32772/CONTENT/ccrsimulation-2.pdf)

[Zenodo ccr simulation](https://zenodo.org/record/6529250#.YpOUmKgpDq4)

[Zenodo caption](https://zenodo.org/record/6561073#.YpDwZagpDq4)

[Archive ccr simulation](https://ia801006.us.archive.org/24/items/ccrSimulation/ccrSimulation-2.pdf)

[OSF ccr simulation](https://osf.io/s5b4u/download)
