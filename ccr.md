### Counterparty Credit Risk


Credit risk is the risk of losses caused by a counterparty or an issuer defaulting on their payment obligations. RiskWatch
provides credit risk functionality to measure credit risk. It focuses on the calculations of credit exposures and capital
allocation based on estimated economic losses. In addition to general credit risk measures (i.e., actual exposure, total
exposure, potential exposure and economic loss), the regulatory credit exposure measurement (BIS methodology) is also
supported.

If one party of a contract defaults, the non-defaulting party will find a similar contract with another counterparty in the market to replace the default 
one. That is why counterparty credit risk sometimes is referred to as replacement risk.

Credit exposure is the amount a bank can potentially lose in the event that one of its counterparties defaults. Note that only OTC deals (and security 
financing transactions) are subject to counterparty risk. We define replacement risk in the context of this report as the maximum of the PFE at a set of 
pre-specified valuation time buckets.

CCR relies on exposure profiles. They are the product of pricing all deals into the future under Monte Carlo simulation and aggregating using all relevant 
netting and collateral agreements. Another important feature that is shared with VaR calculation is the simulation of underlying market factor that is 
required in order to evaluate those deals

Master agreement is a document agreed between two parties, which applies to all transactions between them. Close out and netting agreement is part of 
the Master Agreement. If two trades can be netted, the credit exposure is E(t)=max(V_1 (t)+V_2 (t),0). If two trade cannot be netted (called non-netting), 
the credit exposure is E(t)=max(V_1 (t),0)+max(V_2 (t),0).

CSA (or Margin Agreement or Collateral Agreement) is a legal document that regulates collateral posting. Trades under a CSA should be also under a 
netting agreement, but not vice verse. It defines a variety of terms related to collateral posting: threshold, minimum transfer amount (MTA), independent 
amount (or initial margin or haircut), credit exposure after taking CSA into account.



Reference: 

[ccr](/ccr-1.pdf)

[Zenodo capped frn](https://zenodo.org/record/6558277#.YpDwUqgpDq4)

[Zenodo ccr](https://zenodo.org/record/6529211/files/zenodo-ccr.pdf)

[OSF ccr](https://osf.io/2dg48/download)

[Gitbook ccr exposure](https://cmrm11.gitbook.io/counterparty-exposure/)

[Gitbook ccr stress](https://cmrm11.gitbook.io/counterparty-risk-stress-test/)

[Gitbook ccr measures](https://cmrm11.gitbook.io/counterparty-risk-measure/)

[OSF pooling](https://osf.io/atyb9/download)
