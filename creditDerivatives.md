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



#### Credit Contingent Interest Rate Swap 

The credit contingent interest rate swap (CCIRS or CCDS) valuation model serves the purpose of pricing an option that grants its holder the right, but not the obligation, to enter into an interest rate swap (IRS) at the time when its reference obligor defaults. The premium to be paid on the underlying IRS is fixed in advance at some strike level. The notional amount of the swap is dependent on a predetermined fixed amount and the recovery rate of the reference obligor.  

In essence, a CCIRS trade can be regarded as an interest rate swaption with two special features. One is that the maturity of the swaption is the default time of the reference obligor, which is unknown. The other feature is that, although the strike of the underlying swap is predetermined, the tenor and the notional amount of the underlying swap are dependent on the default time and recovery rate of the reference obligor, respectively. The trade provides a hedging of the counterparty risk in an IRS. 

[Zenodo CCDS pdf](https://zenodo.org/record/7362947/files/ccds.pdf)

[Zenodo CCDS](https://zenodo.org/record/7362947)

[Github CCDS](https://github.com/cfrm17/ccirs)



### CDO Mapping

The model serves the purpose of finding a proxy CDO for a CDO2 or CDO3 trade by matching b/e spread. The proxy CDO has a collateral pool with the same reference names as that of the CDO2 or CDO3 trade and the notional amount of each name is the average of that of all child CDO pools. It has the same thickness of the tranche as that of the CDO2 or CDO3 trade and its attachment is calculated such that the b/e spread matches that of the CDO2 or CDO3 trade. The MTM of the CDO2 or CDO3 trade can then be calculated using the market observed correlations by finding the MTM of the proxy via index base correlations.

The methodology can be illustrated through the following example. As shown in Figure 1, a CDO2 trade has two child pools with the reference names 8~12 being shared. This CDO2 trade can be mapped to another risk equivalent CDO (RE-CDO) with the pool shown in Fig. 1. In this pool the notional of each reference name is the average of that of two child CDOs.  

[Zenodo CDO Mappping  pdf](https://zenodo.org/record/7363084/files/CDOnMapping.pdf)

[Zenodo CDO Mappping](https://zenodo.org/record/7363084)

[Github CDO Mappping](https://github.com/cfrm17/cdoMapping)



### Hazard Rate Curve 

By definition the hazard rate has to be positive to ensure a larger than zero default probability within any period of time. It is a function of credit spread curve, recovery rate, and interest rate.  The credit spread curve is defined as a set of the market quoted CDS spreads with different terms to maturity. We assume one constant recovery rate for each obligor. Normally we assume 0.35 or 0.4 for most of the obligor and 0.15 for subordinate names. 

Given all the input parameters, the hazard rate curve is calculated via bootstrapping. There exists a possibility of failing to building a valid one, either because 1) the input implies a negative hazard rate or 2) a value outside of root finding range. In the GSP model, a root finding scheme is used in which we set the searching range to be 0 and 20.  


[Zenodo Hazard Rate Curve pdf](https://zenodo.org/record/7373116/files/CDSHCurve.pdf)

[Zenodo Hazard Rate Curve](https://zenodo.org/record/7373116)

[Github Hazard Rate Curve](https://github.com/cfrm17/hazardRate)


### Credit Default Swap Option 

The European Credit Default Swap Option (CDSO) pricing model serves the purpose of pricing an option that grants its holder the right, but not the obligation, to enter into a Credit Default Swap (CDS) at some future point in time. The premium to be paid on this forward-start CDS is fixed in advance at some strike level. If the reference entity should default before the forward-start date, the contract is in null and no payments are made.

It is natural to try to value a CDSO by using an approach similar to that of the valuing a European swaption in interest rate markets. It has been proved that a modified Black future pricing closed form solution can be derived to price CDSO, by which the model follows.


[Zenodo CDSO pdf](https://zenodo.org/record/7373465/files/CDSO.pdf)

[Zenodo CDSO pdf](https://zenodo.org/record/7373465)

[Github CDSO pdf](https://github.com/cfrm17/cdso)


### Default Sensitivity

The Risk Engine has two functions: default sensitivity test and credit spread sensitivity test. It is implemented by the Scenario Manager, an autorun program, which manages the calculation of MTM value of the deal and the sensitivity Greeks. 

Default sensitivity test is a kind of stress tests matching the situation that a credit default event of an obligor has occurred or is perceived to be imminent. It is implemented by finding the change of Present Value (PV) for the tranches when the default time of an obligor is perturbed. The Scenario Manager Model is implemented by setting the default time of each obligor to be the valuation date when calculating the present value of each tranche, no matter when that obligor defaults in the generated Monte Carlo (MC) scenarios. 


[Zenodo Default Sensitivity pdf](https://zenodo.org/record/7373904/files/DefaultSensitivity.pdf)

[Zenodo Default Sensitivity](https://zenodo.org/record/7373904)

[Github Default Sensitivity](https://github.com/cfrm17/defaultSensitivity)


### Credit Default Swap Index Curve Adjustment

The purpose of the model is to make adjustment to the credit spread curve of each reference name in the credit default swap (CDS) index portfolio such that the market price of the index can be reproduced using these individual curves. The adjusted index constituent curves are then used to price the standard collateral debt obligation (CDO) tranches based on the index portfolio, which is essential to build a base correlation curve.

Market quoted CDS indices, such as CDX or Tracer-X, are defined as the fair premium paid over a stream of risky coupons in exchange of default protection on standardized portfolios. Unlike a stock index it is not simply the weighted average of credit spreads for the reference names in the portfolio.  A CDS index on a portfolio can be viewed as the b/e spread to an untranched basket credit default swap on that portfolio. As a result, an index position at a level   is equivalent to a portfolio of CDS on the reference names, where all CDSs are entered at the same spread  . Individually, each CDS does not trade at b/e spread, but the portfolio as a whole does. Furthermore, market quoted index assumes a flat credit spread curve and 0.40 recovery rate.

[Zenodo CDS Curve pdf](https://zenodo.org/record/7373680/files/creditCurveAdjustment.pdf)

[Zenodo CDS Curve](https://zenodo.org/record/7373680)








