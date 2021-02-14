
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

A complex solution will use different stochastic processes are used for different risk factors. Different calibration processes apply. 

Simulate yield curve or zero curve represented by yield rates or zero rates rather than swap curve represented by futures and swap rates. There are many 
points in a yield curve, e.g., 1d, 1w, 2w 1m, etc. One can use Principal Component Analysis (PCA) to convert, say, 20 points into 3 point drivers. 
Using PCA, you only need to simulate 3 drivers for each curve. But please remember you need to convert 3 drivers back to 20-point curve at each path 
and each time step.



Reference: 

[CCR Simulation](/ccrSimulation-2.pdf)

[Pub ccr sim](https://interestrate.pubpub.org/pub/uv7fnc6p)

[Pub ccr sim pdf](https://assets.pubpub.org/3d8smglr/51598705809692.pdf)

[Authorstream ccr sim](http://www.authorstream.com/Presentation/tommills-4394407-credit-risk-simulation-methodology/)

[Powershow ccr sim](https://www.powershow.com/view0/90bf56-M2NiY/Credit_Risk_Simulation_Model_powerpoint_ppt_presentation)

[Slideserve ccr sim](https://www.slideserve.com/davidxiao/counterparty-credit-risk-simulation-methodology-powerpoint-ppt-presentation)

[PubHtml5 cva](https://pubhtml5.com/noml/ihcx/basic)

[ScienceMedia cva](http://science-media.org/userfiles/1020/papers/1020_paper_1184.pdf)

[FlipHtml5 ccr simulation](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamkDN4UzM5ITPkl0av9mY)

[Hcommons ccr simulation](https://hcommons.org/deposits/download/hc:32772/CONTENT/ccrsimulation-2.pdf)

[Gitlab ccr simulation](https://gitlab.com/cfrm171/ccrsimulation/-/raw/master/ccrSimulation-2.pdf)

[Bitbucket ccr simulation](https://bitbucket.org/cfrm17/ccrsimulation/downloads/ccrSimulation-2.pdf)

[Github ccr simulation](https://github.com/cfrm17/ccrSimulation/raw/master/ccrSimulation-2.pdf)

[Pubpub ccr simulation](https://interestrate.pubpub.org/pub/tjzhcqez/download/pdf)

[Zenodo ccr simulation](https://zenodo.org/record/4016304/files/ccrSimulation-2.pdf)

[ScienceMedia ccr simulation](http://science-media.org/userfiles/1020/presentations/1020_presentation_433.pdf)

[Archive ccr simulation](https://ia801006.us.archive.org/24/items/ccrSimulation/ccrSimulation-2.pdf)

[OSF ccr simulation](https://osf.io/s5b4u/download)
