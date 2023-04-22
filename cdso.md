
### Credit Default Swap Option 


The European credit default swap option (CDSO) valuation model is employed to price an option that grants its holder the right, but not the obligation, to enter into a Credit Default Swap (CDS) at some future point in time. The premium to be paid on this forward-start CDS is fixed in advance at some strike level. If the reference entity should default before the forward-start date, the contract is in null and no payments are made.

A closed form solution, which is similar to the Black’s model for interest rate swaption, is implemented within the current credit library framework. The forward credit spread of the underlying CDS is computed using pricing model for CDS and the counterparty risk is handled with default correlation model. Apart from pricing, the model can be employed to back out the implied volatility of the forward credit spread.

The European Credit Default Swap Option (CDSO) pricing model serves the purpose of pricing an option that grants its holder the right, but not the obligation, to enter into a Credit Default Swap (CDS) at some future point in time. The premium to be paid on this forward-start CDS is fixed in advance at some strike level. If the reference entity should default before the forward-start date, the contract is in null and no payments are made.

It is natural to try to value a CDSO by using an approach similar to that of the valuing a European swaption in interest rate markets. It has been proved that a modified Black future pricing closed form solution can be derived to price CDSO, by which the model follows.

In the following of the report, we assume the valuation date t, the forward-start date of CDS   (maturity of CDSO), and the forward CDS fixed fee payments at interval   (maturity of CDS). 

The underlying asset of the CDSO is the forward-start CDS.  In order to calculate the forward CDS credit spread, we need first to determine the default probability of the underlying reference entity.  


References:

[zenodo pdf](https://zenodo.org/record/7831646/files/CDSO.pdf)

[archive spread](https://ia803404.us.archive.org/12/items/eq-spread-16/EqSpread-archive.pdf)

[gitbook mortgage](https://finwhite.gitbook.io/mortgagepoolcalculation/)

[github cds](https://github.com/cfrm17/cds)

[osf touch](https://osf.io/6m5jx/download)
