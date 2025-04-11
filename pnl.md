
### Profit and Loss 


Risk measurement will create a strong linkage between pricing models used for profit and loss (P&L) and pricing models used for risk measurement. All market inputs are available for incorporation to risk management systems though some require alternative historical data for calibration procedures. Consistent valuation models will facilitate the identification of market factors driving valuation. 

A revamped Front Office and Middle Office trade and P&L validation process (new “End of Day”) will result in the ability to report T+0 P&L measurement and risk measurement via the Transit Valuator application and accompanying Middle Office reports. This process will provide a linkage between the Actual P&L, Explained P&L, pricing models, and market data. It will also facilitate the identification of trade capture errors and reduce the requirement of VaR proxies.

Market data accuracy will also improve significantly with the common set of pricing models which allows for direct re-use of official valuation market data (sourcing from the Front Office and Global Middle Office databases, and Valuation Product Control group). This will significantly reduce the complexity of managing multiple market data sources. All market data required for daily valuation is to be saved in databases which are accessible to the relevant Market Risk teams. Data used to compute P&L, PAA,  BT and shocks used in VaR should be the same.

The selection of factors may require an evaluation of the simulation modelling under various definitions (such as simulating relative or absolute returns). To the extent that not all market inputs for valuation are represented in the VaR risk factor simulation set, this should be investigated and the justification documented. Often market inputs are rendered more coarse as they are translated to risk factors (i.e. a 27 point yield curve for valuation may be translated to a 5 point yield curve for VaR simulation).  Such translations should also be reviewed and documented as to evidence that the underlying characterization of the market risk is preserved.

With a semi-annual frequency, factors used to decompose P&L for PAA purposes should be compared to risk factors simulated in VaR. PAA involves either 1) a greek-based approach which incorporates changes in PAA market inputs and PAA Greeks or 2) a full revaluation, sequential perturbation of PAA market inputs. In Nextgen, this comparison will be facilitated through common pricing model.


References:

[More details](PnLExplain.pdf)

[archive corporate bond](https://ia601308.us.archive.org/10/items/corporate-bond_202504/CorporateBond.pdf)

[github vol](https://github.com/cfrm17/volInterpolation)

[github xccy](https://github.com/cfrm17/xccySwaption)

[github zero](https://github.com/cfrm17/zeroCouponSwaption)
