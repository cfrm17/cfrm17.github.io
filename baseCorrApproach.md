
### Base Correlation Approach


The model provides five methods to match expected losses and “Loss Ratio” is the proposed one. Test results show that the methodology appears reasonable and has been implemented correctly. Therefore, the GCP base correlation template is approved

The approach implements a base correlation, which is employed to calculate an appropriate correlation in the valuation of a collateral debt obligation (CDO) tranche using market information.  The credit default swaps (CDS) indexes iBoxx and Trac-X portfolios have been introduced in the market and the standard tranches linked to these reference sets are actively quoted. From this market information, we intend to retrieve the correlation information of the standardized collateral pool and then use it to get the market implied correlation for 1) non-standard CDO tranches with standard collateral pools and 2) tranches of a bespoke non-index CDO trade.

The base correlation curve is defined as the correlation inputs required for a series of equity tranches that gives the tranche value consistent with quoted spreads. It was introduced by JPMorgan to address the difficulty of applying market-implied correlation to a tranche with non-standard attachment and detachment points. 

However, as far as we know there is no established methodology to extend this approach to find the implied correlation of a non-index CDO trade, in which the writedown structure, collateral pools, and maturity could be quite different from the market quoted indexes. Some relevant research has tried to bridge the differences between the different standard indexes.

As shown below in this report, five mapping criteria have been implemented in the submitted GCP model. All of them somehow try to match normalized expected losses. It seems reasonable based on the assumption that CDO trades have a similar loss distribution function with a given level of correlation. Based on the testing, “Loss Ratio” is confirmed to be the most appropriate one, which is theoretically consistent to the algorithm of building base correlation curve and more robust for GCP Poisson model.


References:

[zenodo pdf](https://zenodo.org/record/7831616/files/BaseCorrApproach.pdf)

[archive convertible](https://ia803402.us.archive.org/6/items/eq-convertible-4/EqConvertible-archive.pdf)

[gitbook cash](https://finwhite.gitbook.io/mutualfundcashflow/)

[github bond](https://github.com/cfrm17/bondFuturesOption)

[osf cppi](https://osf.io/rcf93/download)
