
### Backtest Exception


Backtest exceptions occur when Clean P&L and/or Model P&L exceed Model VaR on an absolute basis. The use of both model P&L and clean P&L for exception reporting gives granularity in the drivers of the exception as described above.

The backtest P&L calculations are based on the actual day-over-day changes in market inputs observed.  The market inputs must be the same as those used for official valuation thereby establishing a direct linkage to P&L. 

Root cause investigations are required to validate instances of backtest exceptions. Investigation documentation should be prepared, including the root cause, the analysis performed to find the root cause, and the follow-up actions to be taken, if any. 

Comparison of day-over-day market data change with the changes or scenario shocks implied by the VaR scenario can be utilized to validate the exceptions.

Cases where the market move is the only cause of the exception, no further validations are required. The conclusion can be further proved by a comparison of the market data change with its historical trend, showing that the move is in a greater magnitude than the historical data, as well as what’s captured in the VaR window.

Cases where the market move is in line with its historical trend, implying the VaR scenario shocks are relatively benign, the framework around reviewing Model Assumptions can be applied for further investigations. The Risk Measurement Performance Review has responsibility for this examination.


References:

[bitbucket pdf](https://bitbucket.org/timxiao1203/backtest-exception/downloads/BacktestException.pdf)

[github aeco](https://github.com/cfrm17/aecoOption)

[github avg](https://github.com/cfrm17/avgOption)

[github avg strike](https://github.com/cfrm17/avgStrikeOption)
