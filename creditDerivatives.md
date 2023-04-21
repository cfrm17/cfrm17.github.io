## Credit Derivatives


### Base Correlation

The base correlation curve is defined as the correlation inputs required for a series of equity tranches that gives the tranche value consistent with quoted spreads. It was introduced by JPMorgan to address the difficulty of applying market-implied correlation to a tranche with non-standard attachment and detachment points. 

References: 

[Zenodo Base Correlation pdf](https://zenodo.org/record/7831611/files/BaseCorrelation.pdf)

[Zenodo Base Correlation](https://zenodo.org/record/7831611)

[Github Base Correlation](https://github.com/cfrm17/baseCorrelationModel)


### Base Correlation Approach

The approach implements a base correlation, which is employed to calculate an appropriate correlation in the valuation of a collateral debt obligation (CDO) tranche using market information.  The credit default swaps (CDS) indexes iBoxx and Trac-X portfolios have been introduced in the market and the standard tranches linked to these reference sets are actively quoted. From this market information, we intend to retrieve the correlation information of the standardized collateral pool and then use it to get the market implied correlation for 1) non-standard CDO tranches with standard collateral pools and 2) tranches of a bespoke non-index CDO trade.

References: 

[Zenodo Base Correlation Approach pdf](https://zenodo.org/record/7831646/files/CDSO.pdf)

[Zenodo Base Correlation Approach](https://zenodo.org/record/7831646)

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

References

[Zenodo CCDS pdf](https://zenodo.org/record/7362947/files/ccds.pdf)

[Zenodo CCDS](https://zenodo.org/record/7362947)

[Github CCDS](https://github.com/cfrm17/ccirs)

[Researchgate credit](https://www.researchgate.net/profile/Tim-Xiao/publication/337180499_Pricing_Financial_Derivatives_Subject_to_Multilateral_Credit_Risk_and_Collateralization/links/64274b7266f8522c38e94f59/Pricing-Financial-Derivatives-Subject-to-Multilateral-Credit-Risk-and-Collateralization.pdf)



### CDO Mapping

The model serves the purpose of finding a proxy CDO for a CDO2 or CDO3 trade by matching b/e spread. The proxy CDO has a collateral pool with the same reference names as that of the CDO2 or CDO3 trade and the notional amount of each name is the average of that of all child CDO pools. It has the same thickness of the tranche as that of the CDO2 or CDO3 trade and its attachment is calculated such that the b/e spread matches that of the CDO2 or CDO3 trade. The MTM of the CDO2 or CDO3 trade can then be calculated using the market observed correlations by finding the MTM of the proxy via index base correlations.

The methodology can be illustrated through the following example. As shown in Figure 1, a CDO2 trade has two child pools with the reference names 8~12 being shared. This CDO2 trade can be mapped to another risk equivalent CDO (RE-CDO) with the pool shown in Fig. 1. In this pool the notional of each reference name is the average of that of two child CDOs.  


References

[More details](cdoMapping.md)

[Zenodo CDO Mappping  pdf](https://zenodo.org/record/7363084/files/CDOnMapping.pdf)

[Zenodo CDO Mappping](https://zenodo.org/record/7363084)

[Github CDO Mappping](https://github.com/cfrm17/cdoMapping)



### Hazard Rate Curve 

By definition the hazard rate has to be positive to ensure a larger than zero default probability within any period of time. It is a function of credit spread curve, recovery rate, and interest rate.  The credit spread curve is defined as a set of the market quoted CDS spreads with different terms to maturity. We assume one constant recovery rate for each obligor. Normally we assume 0.35 or 0.4 for most of the obligor and 0.15 for subordinate names. 

Given all the input parameters, the hazard rate curve is calculated via bootstrapping. There exists a possibility of failing to building a valid one, either because 1) the input implies a negative hazard rate or 2) a value outside of root finding range. In the GSP model, a root finding scheme is used in which we set the searching range to be 0 and 20.  

References

[Zenodo Hazard Rate Curve pdf](https://zenodo.org/record/7373116/files/CDSHCurve.pdf)

[Zenodo Hazard Rate Curve](https://zenodo.org/record/7373116)

[Github Hazard Rate Curve](https://github.com/cfrm17/hazardRate)


### Credit Default Swap Option 

The European Credit Default Swap Option (CDSO) pricing model serves the purpose of pricing an option that grants its holder the right, but not the obligation, to enter into a Credit Default Swap (CDS) at some future point in time. The premium to be paid on this forward-start CDS is fixed in advance at some strike level. If the reference entity should default before the forward-start date, the contract is in null and no payments are made.

It is natural to try to value a CDSO by using an approach similar to that of the valuing a European swaption in interest rate markets. It has been proved that a modified Black future pricing closed form solution can be derived to price CDSO, by which the model follows.

References

[Zenodo CDSO pdf](https://zenodo.org/record/7373465/files/CDSO.pdf)

[Zenodo CDSO pdf](https://zenodo.org/record/7373465)

[Github CDSO pdf](https://github.com/cfrm17/cdso)

[Researchgate CDS pdf](https://www.researchgate.net/profile/Tim-Xiao/publication/337684918_The_Valuation_of_Credit_Default_Swap_with_Counterparty_Risk_and_Collateralization/links/64274784a1b72772e43efd95/The-Valuation-of-Credit-Default-Swap-with-Counterparty-Risk-and-Collateralization.pdf)


### Default Sensitivity

The Risk Engine has two functions: default sensitivity test and credit spread sensitivity test. It is implemented by the Scenario Manager, an autorun program, which manages the calculation of MTM value of the deal and the sensitivity Greeks. 

Default sensitivity test is a kind of stress tests matching the situation that a credit default event of an obligor has occurred or is perceived to be imminent. It is implemented by finding the change of Present Value (PV) for the tranches when the default time of an obligor is perturbed. The Scenario Manager Model is implemented by setting the default time of each obligor to be the valuation date when calculating the present value of each tranche, no matter when that obligor defaults in the generated Monte Carlo (MC) scenarios. 

References

[Zenodo Default Sensitivity pdf](https://zenodo.org/record/7373904/files/DefaultSensitivity.pdf)

[Zenodo Default Sensitivity](https://zenodo.org/record/7373904)

[Github Default Sensitivity](https://github.com/cfrm17/defaultSensitivity)


### Credit Default Swap Index Curve Adjustment

The purpose of the model is to make adjustment to the credit spread curve of each reference name in the credit default swap (CDS) index portfolio such that the market price of the index can be reproduced using these individual curves. The adjusted index constituent curves are then used to price the standard collateral debt obligation (CDO) tranches based on the index portfolio, which is essential to build a base correlation curve.

Market quoted CDS indices, such as CDX or Tracer-X, are defined as the fair premium paid over a stream of risky coupons in exchange of default protection on standardized portfolios. Unlike a stock index it is not simply the weighted average of credit spreads for the reference names in the portfolio.  A CDS index on a portfolio can be viewed as the b/e spread to an untranched basket credit default swap on that portfolio. As a result, an index position at a level   is equivalent to a portfolio of CDS on the reference names, where all CDSs are entered at the same spread  . Individually, each CDS does not trade at b/e spread, but the portfolio as a whole does. Furthermore, market quoted index assumes a flat credit spread curve and 0.40 recovery rate.

References

[Zenodo CDS Curve pdf](https://zenodo.org/record/7373680/files/creditCurveAdjustment.pdf)

[Zenodo CDS Curve](https://zenodo.org/record/7373680)



### Deferred CDO Coupon Payment 

The model serves the purpose of computing the value of the accumulated coupon payments held in the non-interest-bearing reserve account for a CDO trade [1]. It is a part of the valuation model for a non-vanilla CDO trade called “rated equity”, which is defined as an equity tranche with part of its coupon payments held in a reserve account. 

Modeling the accumulated coupon payments is straightforward within the current structured credit derivative modeling framework. The amount of each coupon payment is calculated the same way as a vanilla CDO trade. Because the reserve account is non-interest-bearing, all the cash flows held in the account are discounted using an appropriate discount factor at the trade maturity. Note that for an interest bearing reserve account, accumulated coupon payments are valued in the same way as that for a vanilla CDO trade and no new model is required.

References

[Zenodo Deferred Payment pdf](https://zenodo.org/record/7374179/files/DeferredPay.pdf)

[Zenodo Deferred Payment pdf](https://zenodo.org/record/7374179)

[Github Deferred Payment](https://github.com/cfrm17/deferredCdsPayment)



### Forward Starting CDO 

There are two advantages of the model. First, like other non-parametric modeling approaches, the model ensures an arbitrage free pricing model once successfully calibrated. Moreover, as shown in the next section, the model can be calibrated to the market information with at least two different maturities, which can be viewed as a progress of the non-parametric modeling. As far as we know, all the other non-parametric modeling can only be calibration to market data with one maturity.

References

[Zenodo Forward CDO pdf](https://zenodo.org/record/7374358/files/FSCDO.pdf)

[Zenodo Forward CDO pdf](https://zenodo.org/record/7374358)

[Github Forward CDO](https://github.com/cfrm17/forwardCdo)



### Forward Starting CDO Model Implementation

The methodology of the model is considered acceptable, based on the fact that the model can be calibrated to the pertinent spot market information with different terms, effectively deal with market implied correlation skew structure, and reasonably model the default events before the forward starting date. However, there are two embedded model uncertainties. One is the calibration process of WMC in which the optimization of hundreds of instruments is involved for a normal FSCDO trade. This task is difficult and it is unlikely to achieve a perfect calibration to all instruments. The selection of the spot calibrating instruments, specially the spot tranches, also contributes to the uncertainties of the calibration.  The other uncertainty resides in the generation of the prior MC scenario. Two different choices would give different prices of the forward trade, even if both can be successfully calibrated to the spot market information. 

References

[Zenodo Forward CDO Implementation pdf](https://zenodo.org/record/7374369/files/FSCDOImplementation.pdf)

[Zenodo Forward CDO Implementation pdf](https://zenodo.org/record/7374369)

[Zenodo Forward CDO Implementation](https://github.com/cfrm17/forwardCdoImplementation)


### Correlation MTM Procedure

Specifically, we examined the proposed procedure for mapping tracer tranches to non-index CDO tranches in a portfolio. The goal of the procedure is to be able to use the tracer market to imply a correlation suitable for marking the market of the CDOs.

We first need to determine an market implied correlation for the tracer tranches. In order to do so, each tranche is valued at various constant correlations ranging from 0 to 0.7 in increments of 0.1. The implied correlation for each tranche is then found by linear interpolation by matching the model price with the market price. Note that this approximation might not be ideal if the market value versus correlation is not linear.

References

[Zenodo Correlation MTM pdf](https://zenodo.org/record/7378011/files/CorrelationMtm.pdf)

[Zenodo Correlation MTM](https://zenodo.org/record/7378011)

[Github Correlation MTM](https://github.com/cfrm17/correlationMtm)



### Credit Derivative Pricing Model

In general the model is within the framework of the multivariate Poisson distribution, in which the default correlation between obligors is introduced solely as a relationship between their hazard rate curves.  

Most credit derivatives structures rely on Monte Carlo (MC) simulation due to the difficulty of obtaining exact closed-form solutions in the manner discussed above.  In particular, the Monte Carlo approach permits the valuation of first-to-default structures taking into account the risk of default of the protection seller.  The general approach taken is the simulation of event times generated by our primitive- and joint-event generators

References

[Zenodo Credit Pricing pdf](https://zenodo.org/record/7832032/files/CreditDerivativePricing.pdf)

[Zenodo Credit Pricing pdf](https://zenodo.org/record/7832032)

[Github Credit Pricing](https://github.com/cfrm17/creditDerivativePricing)



### Credit Pricing Model Calibration

This simple procedure has the effect of normalizing the solution, allowing the solution to recover.  This modification is accompanied by an error-checking condition.  If the solution obtained by the ostrich algorithm does not match the inputs to within a specified tolerance, a failure is reported.

The testing process was carried out in two stages.  First, the independent implementation of the model which was constructed for the testing of the original model outlined in was modified. 

The second phase of the process was carried out using the previous version of the model independently modified to conform to the new specifications by the author to make further tests.  These tests were conducted with both the new implementation of the model and the previous version of the model.

References

[Zenodo Credit Calibration pdf](https://zenodo.org/record/7378454/files/CreditModCorr.pdf)

[Zenodo Credit Calibration](https://zenodo.org/record/7378454)

[Github Credit Calibration](https://github.com/cfrm17/creditPricing)



### Credit Pricing Model Monte Carlo Acceleration

The new method generates small negative delta amounts in certain cases.  Based on the numerical results, these negative deltas are not confined to situations of high correlation and/or large spread differences between credits.  The negative deltas do seem, however,  to be consistent with zero and to therefore be the result of a noise component introduced in certain cases by the acceleration algorithm.

A typical Monte Carlo simulation algorithm assigns each simulation run, or path, an identical probability weight.  If we allow, however, a different probability to be assigned to each simulation path, we allow more flexibility in the simulation and can thus shape the simulation in accordance with our needs.  For example, we can choose the probabilities of each path in manner such that the simulation is guaranteed to reproduce the prices of “benchmark” securities, whose prices are known from market data.  A simulation thus calibrated to benchmarks will then price off-market securities in a realistic manner.

References

[Zenodo Credit Acceleration pdf](https://zenodo.org/record/7832058/files/CreditAcceleration.pdf)

[Zenodo Credit Acceleration](https://zenodo.org/record/7832058)

[Github Credit Acceleration](https://github.com/cfrm17/McAcceleration)



### Implied Correlation of CDO Index Tranche

Because there is no explicit solution for correlation and we employ Monte Carlo simulation (MC) for CDO valuation in model, it is very time consuming to run root finding by iteration. It is also impossible to get an accurate solution due to the presence of MC noise. Hence in the submitted model each tranche is first valued at various constant correlations ranging from 0 to 1 with interval 0.05. The implied correlation for each tranche is then found through linear interpolation by matching the calculated value with the market price.

The main approximation of this methodology is the linear interpolation. As shown in the next section, the tranche value is not a linear function of correlation, especially for mezzanine tranches. Therefore, a non-linearity error will occur.  However, this error could be reduced with increased granularity. Hence the main target is to assess if the correlation change interval (0.05 in the submitted model) is adequate.

References

[Zenodo Implied Correlation pdf](https://zenodo.org/record/7378580/files/ImpliedCorrelation.pdf)

[Zenodo Implied Correlation](https://zenodo.org/record/7378580)

[Github Implied Correlation](https://github.com/cfrm17/impliedCorrelation)



### Implied Base Correlation Mapping Methodology

To our best knowledge there is no generally accepted mapping methodology. It is an open question and subject to future research. Furthermore, several ad hoc adjustments have to be made, if a bespoke tranche is to be calibrated to different indices. This makes it more difficult for the market participants to find a consensus solution to the mapping methodology. In our opinion, the base correlation mapping is theoretically sound only if the risk profile of the bespoke portfolio is similar to that of the indices. For example, if a bespoke portfolio has well-diversified North America names with similar trade definition of the CDX and similar credit spread levels, it would be reasonable to use the base correlation implied by CDX indices.  If they are different, there exist uncertainties with respect to dispersion of credit quality, portfolio diversification, and portfolio mixture issues. No known mapping methodology can fully address all the uncertainties. 

References

[Zenodo Implied Correlation pdf](https://zenodo.org/record/7382668/files/LRMapping.pdf)

[Zenodo Implied Correlation](https://zenodo.org/record/7382668)

[Github Implied Correlation](https://github.com/cfrm17/correlationMapping)


