## Credit Derivatives


### Base Correlation

The base correlation curve is defined as the correlation inputs required for a series of equity tranches that gives the tranche value consistent with quoted spreads. It was introduced by JPMorgan to address the difficulty of applying market-implied correlation to a tranche with non-standard attachment and detachment points. 
References: 

[Zenodo Base Correlation pdf](https://zenodo.org/record/7352577/files/BaseCorrelation.pdf)

[Zenodo Base Correlation](https://zenodo.org/record/7352577)

[Github Base Correlation](https://github.com/cfrm17/baseCorrelationModel)


### Base Correlation Approach

The approach implements a base correlation, which is employed to calculate an appropriate correlation in the valuation of a collateral debt obligation (CDO) tranche using market information.  The credit default swaps (CDS) indexes iBoxx and Trac-X portfolios have been introduced in the market and the standard tranches linked to these reference sets are actively quoted. From this market information, we intend to retrieve the correlation information of the standardized collateral pool and then use it to get the market implied correlation for 1) non-standard CDO tranches with standard collateral pools and 2) tranches of a bespoke non-index CDO trade.

References: 

[Zenodo Base Correlation Approach pdf](https://zenodo.org/record/7352597/files/BaseCorrApproach.pdf)

[Zenodo Base Correlation Approach](https://zenodo.org/record/7352597)

[Github Base Correlation Approach](https://github.com/cfrm17/baseCorrelationApproach)


### Base Correlation Test

As shown in the report, five mapping criteria have been implemented in the submitted model. All of them somehow try to match normalized expected losses. It seems reasonable based 
on the assumption that CDO trades have a similar loss distribution function with a given level of correlation. Based on the testing, “Loss Ratio” is confirmed to be the most 
appropriate one, which is theoretically consistent to the algorithm of building base correlation curve and more robust for Poisson model.

References: 

[Zenodo Base Correlation Test pdf](https://zenodo.org/record/7352694/files/baseCorrelationTest.pdf)

[Zenodo Base Correlation Test](https://zenodo.org/record/7352694)

[Github Base Correlation Test](https://github.com/cfrm17/baseCorrelationExam)