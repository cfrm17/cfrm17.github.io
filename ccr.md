### Counterparty Credit Risk

Counterparty credit risk (CCR) refers to the risk that a counterparty to a bilateral financial derivative contract may fail to fulfill its contractual 
obligation causing financial loss to the non-defaulting party. It will be incurred in the event of default by a counterparty.

Credit risk is the risk of losses caused by a counterparty or an issuer defaulting on their payment obligations. RiskWatch
provides credit risk functionality to measure credit risk. It focuses on the calculations of credit exposures and capital
allocation based on estimated economic losses. In addition to general credit risk measures (i.e., actual exposure, total
exposure, potential exposure and economic loss), the regulatory credit exposure measurement (BIS methodology) is also
supported.

If one party of a contract defaults, the non-defaulting party will find a similar contract with another counterparty in the market to replace the default 
one. That is why counterparty credit risk sometimes is referred to as replacement risk.

Only over-the-counter (OTC) derivatives and financial security transactions (e.g., repo) are subject to counterparty risk. If one party of a contract 
defaults, the non-defaulting party will find a similar contract with another counterparty in the market to replace the default one. That is why 
counterparty credit risk sometimes is referred as replacement risk. The replacement risk is the MTM value of a counterparty portfolio at the time of 
the counterparty default.

Counterparty credit risk measurement is credit exposure (CE). It is the cost of replacing or hedging a contract at the time of default. Other measures 
include Potential future exposure (PFE), Expected exposure (EE), Expected Positive Exposure (EPE), Effective expected exposure (EEE), Effective EPE, 
Exposure at default or EAD. 

If a contract value > 0 to the bank at the time of default, the bank closes out the position and receive nothing from the defaulting counterparty, enter 
a similar contract with another party and pay the contract value. The exposure is the replacement cost, i.e., the contract value. 

If the contract value < 0 at the time of default, the bank closes out the position and paying contract value to the defaulting counterparty, enter a 
similar contract with another party and receives the contract value. The net loss is zero and ete credit exposure can be expressed as E(t) = max(V(t), 0)

Master agreement is a document agreed between two parties, which applies to all transactions between them. Close out and netting agreement is part of 
the Master Agreement. If two trades can be netted, the credit exposure is E(t)=max(V_1 (t)+V_2 (t),0). If two trade cannot be netted (called non-netting), 
the credit exposure is E(t)=max(V_1 (t),0)+max(V_2 (t),0).

CSA (or Margin Agreement or Collateral Agreement) is a legal document that regulates collateral posting. Trades under a CSA should be also under a 
netting agreement, but not vice verse. It defines a variety of terms related to collateral posting: threshold, minimum transfer amount (MTA), independent 
amount (or initial margin or haircut), credit exposure after taking CSA into account.



Reference: 

[ccr](/ccr-1.pdf)

[Zenodo capped frn](https://zenodo.org/record/6558277#.YpDwUqgpDq4)

[FlipHtml5 ccr](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamIDN4UzM5ITPkl0av9mY)

[Hcommon ccr](https://hcommons.org/deposits/download/hc:32754/CONTENT/ccr-1.pdf)

[Zenodo ccr](https://zenodo.org/record/6529211#.YpOUF6gpDq4)

[ScienceMedia ccr](http://science-media.org/userfiles/1020/presentations/1020_presentation_432.pdf)

[Archive ccr](https://ia600105.us.archive.org/18/items/alex_Ccr/ccr-1.pdf)

[OSF ccr](https://osf.io/2dg48/download)


