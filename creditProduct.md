## Credit Proucts


### Loss Trigger Leveraged Super Senior Tranche 

The valuation of LT-LSS trades has been a challenging task in both the industry and academia. LSS trades are essentially exotic options on the forward starting super senior tranche conditional on the trigger breach, which depends on the way how the correlated default events, credit spread of each reference obligor, and market implied correlations evolve over time. The exercise of a LSS trade is contingent on the trigger breach, which can happen at any time before the trade maturity. The value of the trade cannot be fully determined unless a dynamic process of the portfolio is modeled. Furthermore, compared with other triggers, the LT-LSS is the most complicated because it directly links the credit spread and the implied correlation movements to the default events of the collateral pool. It is almost impossible to get pertinent market information to calibrate such a conditional loss process, even if we can somehow model one. The base correlation curve is defined as the correlation inputs required for a series of equity tranches that gives the tranche value consistent with quoted spreads. It was introduced by JPMorgan to address the difficulty of applying market-implied correlation to a tranche with non-standard attachment and detachment points. 

References: 

[Zenodo Loss Trigger pdf](https://zenodo.org/record/7382842/files/LSSWMC.pdf)

[Zenodo Loss Trigger](https://zenodo.org/record/7382842)

[Github Loss Trigger](https://github.com/cfrm17/lossTrigger)


### MezzMezzMezz Trade 

The MezzMezzMezz or Mezzcubed trade model implements a trade structure in which the tranches defined by MezzOfMezz or Caribou structures are aggregated under a new Collateral Debt Obligation (CDO) structure. The synthetic CDO trade models used by the  system are FirstLoss, MezzOfMezz, and MezzMezzMezz. The following diagrams show how these models are structured*.

References:

[Zenodo MezzMezzMezz pdf](https://zenodo.org/record/7383005/files/MezzMezzMezz.pdf)

[Zenodo MezzMezzMezz](https://zenodo.org/record/7383005)

[Github MezzMezzMezz](https://github.com/cfrm17/mezzCubed)


### Normal Copula 

The model implements the normal copula which is a default correlation model. Implemented by Monte Carlo (MC) simulation, the model generates correlated default events of a collateral pool of obligors, hence can be used to value basket default swaps and Collateral Debt Obligations (CDOs) (nofm basket, FirstLoss, Caribou, and MezzMezzMezz). 

The normal copula function is a multi-variate cumulative normal distribution with correlation matrix  . Applying the normal copula function to the modeling of correlated default events of a collateral asset pool, the uniform random variables are mapped to the default probabilities with standard normal distribution. The normal copula function, or the cumulative joint default probability for the collateral pool with n assets

References:


[Zenodo Normal Copula pdf](https://zenodo.org/record/7383168/files/NormalCopula.pdf)

[Zenodo Normal Copula](https://zenodo.org/record/7383168)

[Github Normal Copula](https://github.com/cfrm17/normalCopula)



### Credit Derivative Model

The model serves the purpose of pricing and calculating sensitivities for all credit derivative products, which are Credit Default Swaps (CDSs), First-to-Default swaps (FTDs), FirstNofM basket default swaps (FNMs),  all level Collateral Debt Obligations (CDOs, CDO2s, and CDO3s), and forward starting CDOs. 

References:

[Zenodo Credit Model pdf](https://zenodo.org/record/7383244/files/creditDerivatives.pdf)

[Zenodo Credit Model pdf](https://zenodo.org/record/7383244)

[Github Credit Model](https://github.com/cfrm17/creditDerivatives)



### Giant First Loss Model

Within the existing modeling framework, the trade is implemented by resetting generated default times in each Monte Carlo (MC) scenario to be the maturity date. Compared with the standard first loss trade model, two trends of change can be perceived. First, when the hazard rate of the obligor becomes smaller, the B/E spreads for both models would converge to zero. Second, because in the new model the cash flow pattern for default events has changed, the sensitivity to the interest rate should be different. Generally the new model is not only more sensitive to the interest rate but the sensitivity to its term structure changes dramatically as well. 

First, the sensitivity to the interest rate for the new model and the standard first loss model is compared. The results are shown in Table 2 with the detail results listed in Appendix II. Delta with 5bps parallel shift is calculated by giving a 5bps parallel up shift to the interest rate. Delta with 5bps tilt is computed by giving a 5bps tilt to the interest rate (clockwise tilt within 5 years).

References:

[Zenodo First Loss Model pdf](https://zenodo.org/record/7386972/files/PayEndGiantFirstLoss.pdf)

[Zenodo First Loss Model](https://zenodo.org/record/7386972)

[Github First Loss Model](https://github.com/cfrm17/firstLoss)



### Basket Default Swap 

Within the modeling framework, the sensitivities measure the change of present value (PV) when certain risk factor is perturbed. For example, recovery rate sensitivity is calculated by perturbing the recovery rate for each obligor in the reference collateral pool of the trade, which can be defined as follow.  Assume the collateral pool be a set of obligors,  , in which each obligor is associated with market implied recovery rate  . Base on this collateral pool, a CDO trade has a tranche structure with m tranches,  .  

References:

[Zenodo Basket Default pdf](https://zenodo.org/record/7387516/files/basketDefault.pdf)

[Zenodo Basket Default pdf](https://zenodo.org/record/7387516)

[Github Basket Default](https://github.com/cfrm17/basketDefault)



### Variable Maturity CDO 

Instead of attempting to solve this complicated modelling problem, a simple and flexible approach is adopted in the submitted model. Although it is unpredictable how the portfolio will evolve over time and what the substitution asset would be, it is expected that the substitution asset should have certain probability of default before the trade maturity.  In a MC scenario in which the substituted asset survives beyond its maturity, a default time of the substitution asset is then simulated by assuming that it is forward starting at the time of substitution. The uncertainty in modelling the asset substitution is cushioned by an appropriate model risk reserve, which has been set up by a joint effort 

References:

[Zenodo Variable Maturity CDO pdf](https://zenodo.org/record/7387723/files/VariableMatCDO.pdf)

[Zenodo Variable Maturity CDO](https://zenodo.org/record/7387723)

[Github Variable Maturity CDO](https://github.com/cfrm17/variableCdo)



### Variable Maturity GiantFirstLoss Trade 

The valuation model serves the purpose of pricing a variable maturity GiantFirstLoss trade. The trade has a non-vanilla collateral debt obligation (CDO) structure, in which the maturities of the underlying obligors could be different from that of the CDO trade 

The losses associated with the defaulted obligors are allocated to each tranche according to the subordination of the tranche. In the variable maturity GiantFirstLoss trade as well as this loss claiming scheme, a pay down scheme of the tranches, associated with the reduction of the collateral pool due to the default events and the early retirement events of the obligors, is implemented.  

References:

[Zenodo Variable First Loss pdf](https://zenodo.org/record/7387866/files/VariMatGiantFirstLoss.pdf)

[Zenodo Variable First Loss pdf](https://zenodo.org/record/7387866)

[Github Variable First Loss](https://github.com/cfrm17/variableFirstLoss)



### Weighted Monte Carlo Sensitivity 

The model serves the purpose of computing MTM and risk for the trades priced using weighted Monte Carlo simulation (WMC) model [3].  The WMC model is a non-parametric approach to value complex CDO structures that need to be priced using the market information of the tranche losses at multiple maturities. At the present time, the model is used for the valuation of forward starting CDO trades (FSCDO) and loss-trigger leverage super senior tranches (LT-LSS). 

Three components of the model are submitted. One is a new method of computing sensitivities of the risk factors that can be expressed as a function of the calibrating instruments. Specifically they are credit spread sensitivity and correlation sensitivity for FSCDO trades and LT-LSS trades.  Compared with the old method, which is the shock-recalibration-revaluation of the risk factor, the new method is more efficient and more robust 

References:

[Zenodo Mc Sensitivity pdf](https://zenodo.org/record/7387897/files/McSen.pdf)

[Zenodo Mc Sensitivity pdf](https://zenodo.org/record/7387897)

[Github Mc Sensitivity](https://github.com/cfrm17/mcSen)



### Credit Default Swap Index Basis Adjustment

The implementation of the submitted model was first verified by testing against an independently developed test model. The implications of underlying assumptions in the model were tested against several benchmark models. The internal error tolerance control in the bootstrapping and the choice of the flat term nodes of the indexes were assessed and found appropriate as well.

It is important to note that, from the viewpoint of mathematical modeling, there are many ways to make such adjustments and the methodology of adjustment is only one of the choices. Each choice bears different assumptions on the embedded index basis risk and, to our best knowledge to date, there is no generally accepted market convention of making such adjustment. The test results indicate that, as far as the calibration of the base correlation and the valuation of an index CDO trade are concerned, the differences among those choices are immaterial. It is also indicated that the differences mainly resides in the term nodes that are far from the index maturities, which may be material depending on the hedging strategy for index CDO trades.

References:

[Zenodo Basis Adjustment pdf](https://zenodo.org/record/7387930/files/basisAdjustment.pdf)

[Zenodo Basis Adjustment](https://zenodo.org/record/7387930)

[Github Basis Adjustment](https://github.com/cfrm17/cdsBasisAdjustment)



### Risk Measures for FNM and CDO2&3 Trades

A new method of computing the credit spread sensitivity, namely semi-analytic Monte Carlo (MC) sensitivity, is adopted in the submitted model. It applied to FNM trades and CDO2&3 trades. In the computation of risk, now it is known that a default event that passes across the maturity in the perturbed scenario has a large contribution. Using a usual bump/revaluation approach, it is very hard to model such an event if the perturbation is tiny in the case such as computing CSPDH. In the new model, a deterministic part is added to directly address this part of contribution to credit spread sensitivities; hence the computational efficiency and precision are greatly improved.  

The CSPDH of CDO2&3 trades is the most complicated model in the Oscar/Fritz credit library.  In the model, a CDO2&3 trade is flattened to a risk equivalent vanilla CDO trade (RE-CDO) and then valued within the base correlation framework. When the credit spread of an obligor is perturbed, the attachment point of the RE-CDO trade is changed, which can be found through a re-flattening process. Using the analytical sensitivity approach, the computation of CSPDH for a CDO2&3 trade is decomposed into two parts. One is CSPDH for RE-CDO, which is the same as that of a bespoke trade. The other part is CSPDH attributed to change of the attachment of RE-CDO. This part is calculated via a Jacobian of the attachment point to the credit spread change, in which the analytical MC sensitivity is employed. The first part of CSPDH can be tested straightforwardly by switching off re-flattening option and benchmarking against the approved bespoke CDO pricing template.  We focus on the second part of CSPDH for CDO2&3 trades. 

References:

[Zenodo Risk Measures pdf](https://zenodo.org/record/7387976/files/RiskMeasureFnmCDO2%263.pdf)

[Zenodo Risk Measures](https://zenodo.org/record/7387976)

[Github Risk Measures](https://github.com/cfrm17/riskMeasureCdo)



### Risk Measures for Index Tranches and Bespoke CDOs

The new components developed in the Oscar/Fritz credit library enable us to capture risk more accurately. Previously, the index basis adjustment, base correlation calibration, and CDO2&3 trade equivalent CDO re-flattening (RE-CDO) were implemented outside the Oscar/Fritz library and there was no way to make corresponding adjustments in perturbed scenarios. In the new model, we can recalculate the basis adjustments, remap base correlations, and re-flatten RE-CDOs in the perturbed scenario. 

The credit spread sensitivity is switched to a bucketed one (CSPDH). In the model, parallel shift credit spread sensitivity has been used for many years. However, recent development in the market, especially the popularity of longer term trades, makes this measure inaccurate.

References:

[Zenodo Bespoke pdf](https://zenodo.org/record/7388002/files/RiskMeasuresIndexBespoke.pdf)

[Zenodo Bespoke](https://zenodo.org/record/7388002)

[Github Bespoke](https://github.com/cfrm17/indexRiskMeasure)



### Repo Curve

A repo curve is defined as an adjustment to the discount curve in the pricing of a bond/FRN, when the credit default swaps (CDS) market implied default probability of the issuer is used in the pricing. We have changed the repo curve generation methodology. 

Instead of a fixed term structure, the repo curve for each issuer in essence becomes “repo collections” in which a constant repo factor is stored with respect to each outstanding bond with same issuer. The computation of the repo factor for each bond remains unchanged. 

References:

[Zenodo Repo Curve pdf](https://zenodo.org/record/7428850/files/RepoCurve.pdf)

[Zenodo Repo Curve](https://zenodo.org/record/7428850)

[Github Repo Curve](https://github.com/cfrm17/repoCurve)



### Credit Delta and Credit VaR Measures

Credit default swaps may terminate prior to maturity if the obligor defaults.  The effective duration of a credit default swap is therefore shorter than the term of the swap due to the possibility of swap termination prior to maturity.  The current methodology overstates PV01 values because it does not incorporate the default probability.

Credit spread information derived from debt securities is only an approximation to the swap spread data and may not truly reflect the level and volatility of swap spreads.  Therefore credit spreads of debt securities should only be used as a proxy in the absence of historical spread data for asset swaps and default swaps.  

References:

[Zenodo Credit Delta VaR pdf](https://zenodo.org/record/7473670/files/CreditDeltaVaR.pdf)

[Zenodo Credit Delta VaR](https://zenodo.org/record/7473670)

[Github Credit Delta VaR](https://github.com/cfrm17/creditDeltaVaR)


### Model Reserve

The marked-to-market  (MTM) value of a CDO or FTD baskets can be represented as a function of the market spreads, market liquidity and underlying pricing model (which itself is dependent on the correlation engine and estimated correlation parameters).  Thus, the change in MTM can result from the change in either for the above-mentioned variables.

From the above mathematical representation, the reserves are subject to one main source of model risk – choice of default correlation model. The current reserves amounts are model dependent but the conservative approach to the computation of these reserves will partially encompass model risk.  In order to compute model risk reserves, an alternative generally used model (referred to as the alternative model in this policy) must be available for comparison. The following methodology and process will be used for computing model risk reserves.   

References:

[Zenodo Model Reserve pdf](https://zenodo.org/record/7473768/files/ModelReserves.pdf)

[Zenodo Model Reserve](https://zenodo.org/record/7473768)

[Github Model Reserve](https://github.com/cfrm17/modelReserve)



### Weighted Monte Carlo Simulation

The technique of assigning probability weights has, at least theoretically, the additional benefits of accelerating the convergence of the simulation, as well as allowing the sensitivities of the simulated price with respect to the benchmark securities to be computed without performing additional simulations. 

Sometimes WMC fails to predict a “correct” value for an outstanding trade. According to the theory of WMC, we could not expect the difference between the regular MC simulation and WMC to be so large.

References:

[Zenodo Model Reserve pdf](https://zenodo.org/record/7474236/files/WeightedMc.pdf)

[Zenodo Model Reserve](https://zenodo.org/record/7474236)

[Github Model Reserve](https://github.com/cfrm17/weightedMc)