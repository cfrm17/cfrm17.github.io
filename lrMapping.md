
### Implied Base Correlation Mapping 


The Mapping model serves the purpose of finding implied base correlations for a bespoke CDO trade from market quoted standard CDO indices Dow Jones CDX and iTraxx Europe. In this report, a CDO tranche is defined as bespoke if its reference portfolio composition is different from that of CDO indices.  

A simplified Loss Ratio method (named “Maturity Loss Ratio”) is adopted in the model.  The detachment points of the bespoke base tranche are solved such that, given the same correlation value, the normalized expected losses of the bespoke tranche meet with that of the standard index base tranches. The new method is considered as a replacement of the existing mapping methodology “Scale” to reflect the latest development of credit market. 

To our best knowledge there is no generally accepted mapping methodology. It is an open question and subject to future research. Furthermore, several ad hoc adjustments have to be made, if a bespoke tranche is to be calibrated to different indices. This makes it more difficult for the market participants to find a consensus solution to the mapping methodology. In our opinion, the base correlation mapping is theoretically sound only if the risk profile of the bespoke portfolio is similar to that of the indices. For example, if a bespoke portfolio has well-diversified North America names with similar trade definition of the CDX and similar credit spread levels, it would be reasonable to use the base correlation implied by CDX indices.  If they are different, there exist uncertainties with respect to dispersion of credit quality, portfolio diversification, and portfolio mixture issues. No known mapping methodology can fully address all the uncertainties. 

As an effective way of managing the imbedded uncertainties, the mapping methodology can be monitored through a monthly IPV process. On the other hand no matter what mapping methodology is being used, an adequate model risk reserve has to be set up.

The implementation of the submitted model was first verified by an independently implemented test model. The “Maturity Loss Ratio” and “Loss Ratio” were tested. The underlying approximation of “Maturity Loss Ratio” was assessed. The results were also analyzed. 

The implication of the mapping methodology on MTMs, credit spread sensitivities, default sensitivities, correlation sensitivity, credit spread hedging, and stress testing were investigated. The testing results indicate that, when we switch a mapping methodology, not only MTM will change, but also the hedging positions need to be adjusted which might be costly. Furthermore, a possible mis-hedge can be material, especially in the stress events. In our opinion, adequate IPV/model risk reserve can cover the MTM adjustment. Other risk control methods, such as stress testing and DS-CS gap control, can play an important role to prevent a possible large mis-hedging incurred by the uncertainty of the model.

We therefore concluded that the bespoke mapping methodology “Maturity Loss Ratio” in submitted model is approved for computing mapped base correlations for bespoke CDO trades, conditional on an adequate model risk reserve and a frequent re-review through MarkIt. The old mapping methodology “Scale” is now considered obsolete. 


References:

[zenodo pdf](https://zenodo.org/record/7382668/files/LRMapping.pdf)

[archive himalaya](https://ia803400.us.archive.org/13/items/eq-himalaya-25/EqHimalaya-archive.pdf)

[gitbook cash](https://finwhite.gitbook.io/mortgagecashflow/)

[github basis](https://github.com/timxiao1203/MoneyMarketBasisCurve)

[github bond](https://github.com/timxiao1203/MunicipalBondOption)
