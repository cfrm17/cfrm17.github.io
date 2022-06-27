
### Counterparty Credit Risk Simulation Methodology

Counterparty credit risk (CCR) is the risk of loss that will be incurred in the event of default by a counterparty. It will be incurred in the event of 
default by a counterparty. Only over-the-counter (OTC) derivatives and financial security transactions (e.g., repo) are subject to counterparty risk. 
If one party of a contract defaults, the non-defaulting party will find a similar contract with another counterparty in the market to replace the 
default one. That is why counterparty credit risk sometimes is referred as replacement risk. The replacement risk is the MTM value of a counterparty 
portfolio at the time of the counterparty default.

Counterparty credit risk measure is credit exposure. As credit exposures in future are stochastic, one needs to simulate market evolution in order 
to quantify CCR. This presentation provides some details about CCR simulation.

To calculate credit exposure or replacement cost in future times, one needs to simulate market evolutions. Simulation must be conducted under the 
real-world measure. One could use a simple but inaccurate solution, or accurate but complex approach. Some vendors and institutions use this simplified 
approach. Only a couple of stochastic processes are used to simulate all market risk factors. They use Vasicek model for all mean reverting factors
dr=k(θ-r)dt+σdW where r – risk factor; k – drift; θ – mean reverse; σ – volatility; W – Wiener process. And use Geometric Brownian Motion (GBM) for all 
non-mean reverting risk factors: dS=μSdt+σSdW. The calibration results for different risk factors are different from each other.

There are two main components in calculating credit exposures: scenario generation and instrument valuation. The scenario generation uses Monte Carlo 
simulation to generate the future scenarios of various market risk factors at different future time buckets. Future market scenarios are usually generated 
using “real world measure” instead of “risk-neutral” measure used in pricing. Exposure calculation also requires a valuation methodology to calculate 
consistently the value of a deal over different time bucket in the future. 

The simulation time buckets used by most banks to calculate credit exposure usually have daily or weekly interval up to a month, then monthly up to a year 
and yearly up to five year. The rationale is that as we valuate the deal farther into the future, the exposure calculation becomes less accurate due to the 
accumulated error from simulation discretization, and inherited errors from calibration of the underlying models, such as those due to the change of 
macro-economic climate. The time bucketing scheme used in our project is consistent with the above practice.

Reference: 

[CCR Simulation](/ccrSimulation-2.pdf)

[Zenodo ccr simulation](https://zenodo.org/record/6529250#.YpOUmKgpDq4)

[Zenodo caption](https://zenodo.org/record/6561073#.YpDwZagpDq4)

[Archive ccr simulation](https://ia801006.us.archive.org/24/items/ccrSimulation/ccrSimulation-2.pdf)

[OSF ccr simulation](https://osf.io/s5b4u/download)

[Bitbook add-on exposure](https://cmrm11.gitbook.io/add-on-exposure/)

[Bitbook intraday](https://cmrm11.gitbook.io/intraday-replacement-risk/)