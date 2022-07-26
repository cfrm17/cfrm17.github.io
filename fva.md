
### Funding Valuation Adjustment

Funding Valuation Adjustment (FVA) is introduced to capture the incremental costs of funding uncollateralized derivatives. It can be referred to as the 
difference between the rate paid for the collateral to the bank’s treasury and rate paid by the clearinghouse. Also FVA can be thought of as a hedging 
cost or benefit arising from the mismatch between an uncollateralized client trade and a collateralized hedge in the interdealer market. FVA should be 
also calculated at portfolio level.

FVA is the cost of funding that is considered in the valuation of uncollateralized derivatives. It is introduced to quantify the adjustment to the 
value of derivatives in order to ensure that a trader recovers funding costs that are consistent with the market’s view of the funding costs associated 
with the same trade. This presentation elaborates an integrated framework for calculating both CVA and FVA. We also discuss the pros and cons of comparing 
the popular credit exposure approach and the more accurate least square Monte Carlo approach. 

Both FVA and CVA are computed on the basis of counterparty portfolio that need to take master agreement and collateral agreement into account. 
Master agreement is a document agreed between two parties, which applies to all transactions between them. Close out and netting agreement is part of 
the Master Agreement. If two trades can be netted, the credit exposure is E(t)=max(V_1 (t)+V_2 (t),0). If two trade cannot be netted (called non-netting), 
the credit exposure is E(t)=max(V_1 (t),0)+max(V_2 (t),0).

For some counterparties with bond data from Bloomberg or other approved sources, if there are more than a number bonds available for building the whole term structure 
of the bond spread curve for the counterparty, the bond spread curve is built using the bond yields over the USD swap curve directly with linear interpolation for the 
missing terms.  

If there are not enough number of bonds for a counterparty to build the whole term structure of  bond spread curve, the bond spread curve is built using a hybrid method 
which is to calculate the bond spreads for the available bonds using the bond yields from the data source and interpolate the curve using the generic bond spread curves 
built using the method described below.


Reference: 

[Funding Valuation Adjustment](/cvaFva-5.pdf)

[Zenodo arrear fra](https://zenodo.org/record/6578408/files/arrearFra.pdf)

[Zenodo fva](https://zenodo.org/record/4017723/files/cvaFva-5.pdf)

[OSF fva](https://osf.io/r6y2h/download)

[Github quanto cms](https://github.com/timxiao1203/QuantoCmsSpreadSwap)

[Github inflation swap](https://github.com/timxiao1203/InflationSwap)

[OSF gic](https://osf.io/tgd82/download)
