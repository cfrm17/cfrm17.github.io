
### Delta Gamma Vega Value at Risk

The Delta Gamma Vega (DGV) methodology is developed to estimate Value-at-Risk (VaR) for portfolios of equities and equity options in order to comply, in regard to market risk measurement. The model can accurately estimates over-night VaR for portfolios with non-zero convexity or linear risk.

The DGV methodology assumes that the log-relative changes in equity-prices, implied volatilities, and interest-rates are normally distributed. The method also uses linear regression to describe stock returns in terms of market index returns (CAPM) to reduce the dimension of the variance-covariance matrix and to capture stock specific risk. 

We compute VaR for the following portfolios when Dt =1/250 years.

Portfolio I: 1 stock and 0 options
Portfolio II: 4 stocks and 0 options
Portfolio III: 1 stock and 2 options with no hedges
Portfolio IV: 1 stock and 1 option where delta is hedged
Portfolio V: 1 stock and 2 options where delta, gamma, and vega are hedged
Portfolio VI: 1 stock and 5 options where delta, gamma, vega, rho, and theta are hedged.

When a sensitivity is “hedged” it means that the sensitivity is zero. For example, in Portfolio IV where delta is hedged, this means that the delta of this portfolio is identically zero. The options used in the various portfolios and distributional assumptions are given in appendices 2 and 3, respectively.

The re-implementation part of the testing is used to establish VaR benchmarks that the DGV methodology must agree with. The Monte Carlo part of the testing is used to measure the impact of sensitivities not captured by the DGV methodology. For example, the DGVRT approximation omits terms 

The DGV methodology does not capture the sensitivity in the change in portfolio value whereas the Monte Carlo method accounts for this sensitivity and all others. The Monte Carlo VaR estimates should show large deviations from the DGV VaR estimates for portfolios V and VI because an most of the DGVR sensitivities are perfectly hedged in these portfolios.


References:

[archive pdf](https://ia904701.us.archive.org/30/items/dgv-va-r/DgvVaR.pdf)

[gitbook](https://finwhite.gitbook.io/dgvvar/)

[github carc lockin](https://github.com/cfrm17/carcLockIn)

[core bond pdf](https://core.ac.uk/download/534868157.pdf)

[core worst](https://core.ac.uk/works/126062267)

