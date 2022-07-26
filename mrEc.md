
### Market Risk Economic Capital 

Financial business is exposed to many types of risks due to the nature of business. To guard against the risk, financial institutions must hold capital 
in proportion to the potential risk. Market risk economic capital is intended to capture the value change due to changes in market risk factors. It is 
an internal capital reserve to cover unexpected loss due to market movement. 

Economic capital falls into the category of Value at Risk (VaR) measures as both try to capture value change due to market movement. Most institutions use the 
existing VaR system to compute economic capital. VaR captures the market risk of 1-day time period at 99% confidence level whereas Economic capital measures the 
market risk of 1-year time period at 99.95 confidence level. Therefore, scaling methodology is the key to compute economic capital, i.e., scaling 1-day to 1-year 
and 99% to 99.95%. This presentation is intended to answer several fundamental economic capital questions: what is economic capital? What is the difference 
between economic capital and regulatory capital? How to compute economic capital? 

Economic capital is an internal measure for internal risk control purpose. It is statistically measured for 1-year time period at 99.95% confidence level 
(consistent with the probability of default (0.05%) targeted by most institutions), while regulatory capital is an external measure used by regulators, 
that is statistically measured for 10-day time period at 99% confidence level.

The simplest and most common used time horizon scaling approach is to scale 1-day VaR to 1-year VaR as 1-year VaR at 99% confidence level = √T * 1-day 
VaR at 99% confidence level, where T = 365 for accounting for calendar days only or T = 250 for accounting for business days only. The assumption of 
using this scaling formula is that 1-day portfolio loss distribution is independent and identically distributed (IID), constant mean and volatility,
and no autocorrelationl. This scaling approach is most likely under-estimated risk given the assumptions don’t match the reality.

The methodology of scaling Var to calculate the equivalent portion of Economic Capital is developed reviewed within the team.  The algorithm of combining all
components (stress-based economic capital, equivalent scaled Var, Limit usage at Tier 3 level and Stop-loss limit) to derive the final economic capital is proposed. 
Sample results for some selected desks are prepared jointly with the Limit work stream.  


Reference: 

[Market Risk Economic Capital](/mrEc-11.pdf)

[OSF mrec](https://osf.io/fdmb4/download)

[Zenodo closeout reserve](https://zenodo.org/record/6585388/files/closeOutReserve.pdf)

[Github basis](https://github.com/timxiao1203/MoneyMarketBasisCurve)

[Github bond option](https://github.com/timxiao1203/MunicipalBondOption)

[Zenodo capital](https://zenodo.org/record/6529472/files/Zenodo-mrEc.pdf)

[OSF forward starting](https://osf.io/37fbt/download)
