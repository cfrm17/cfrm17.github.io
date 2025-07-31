
## Market Risk

References:

[Hcommons](https://derivatives.hcommons.org/2023/03/24/market-risk/)


### Market Risk Flow

In the Risk Measurement Data Flow, positions are valued using models and market inputs. The valuation process is enhanced via Independent Price Valuation (IPV), Valuation Adjustments (VA) and proxy bookings. The valuation process then feeds profit and loss (P&L) and Risk which can be connected through the P&L Attribution (PAA). Market risk measures and diagnostics, such as VaR, are an outcome from the risk measures. This forms the cornerstones of the Market Risk Measurement Management and Data Review Process.

The Market Risk Measurement Management and Data Review Process establishes the linkages which are required in an effective risk management system. All data composing these linkages can theoretically trace dependencies back to market inputs and position inputs. Market inputs are defined as the inputs required in the valuation model that are dynamic in nature and are sourced from markets. As an input to the risk process, the positions require thorough review and validation processes to ensure completeness and consistency. The set of inputs required for valuation should also be employed for other calculations such as P&L attribution (PAA) and should be simulated when computing Value at Risk (VaR).


References: 

[More details](riskFlow.md)

[Researchgate variance swap](https://www.researchgate.net/profile/Tim-Xiao/publication/369907899_Variance_Swap_Model/links/6433107420f25554da1d49fb/Variance-Swap-Model.pdf)



### Profit and Loss Explanation

Market data accuracy will also improve significantly with the common set of pricing models which allows for direct re-use of official valuation market data (sourcing from the Front Office and Global Middle Office databases, and Valuation Product Control group). This will significantly reduce the complexity of managing multiple market data sources. All market data required for daily valuation is to be saved in databases which are accessible to the relevant Market Risk teams. Data used to compute P&L, PAA,  BT and shocks used in VaR should be the same.

The identification and selection of market risk factors to be captured in a risk model, such as VaR, are critical to building strong risk measurement platform. The Risk Management Completeness Review Stream will be responsible for regular validation of the risk factors. Risk factors are market variables which are expected to impact valuation P&L. In VaR, “risk factors” also define the returns which are simulated and subsequently mapped to market instruments. 


References: 

[More details](pnl.md)

[Researchgate hedge fund](https://www.researchgate.net/publication/378435843_A_Model_for_Estimating_Daily_Hedge_Fund_Net_Asset_Value/fulltext/65d93fa5c3b52a1170f26ef9/A-Model-for-Estimating-Daily-Hedge-Fund-Net-Asset-Value.pdf)


### Backtest Exception

The backtest P&L calculations are based on the actual day-over-day changes in market inputs observed.  The market inputs must be the same as those used for official valuation thereby establishing a direct linkage to P&L. 

Root cause investigations are required to validate instances of backtest exceptions. Investigation documentation should be prepared, including the root cause, the analysis performed to find the root cause, and the follow-up actions to be taken, if any. 

Exceptions may be classified as legitimate, or false. For instances where the exceptions are deemed as false, such as spurious market data input, and IT system issues, appropriate operational procedures need to be followed for issue resolution including reruns, market data 


References: 

[More details](backtestEx.md)

[Researchgate IR term](https://www.researchgate.net/profile/Tim-Xiao/publication/385275783_Modeling_Term_Structure_of_Cross-_Currency_Interest_Rates/links/671d479dacba566ad501e638/Modeling-Term-Structure-of-Cross-Currency-Interest-Rates.pdf)



### Independent Price Verification

VPC holds a month-end meeting to review all IPV/VA with representatives from the line of business (LOB), Capital Markets Finance, Chief Accountant’s Group, and Risk Oversight. A report is distributed outlining the IPV and VA balances and month over month changes. Detailed reports for each LOB are also available.

VPC will identify material IPV and VA balance for each portfolio (as defined by a unique limit letter) that have a potential impact on VaR. Materiality will be set at total IPV adjustment or total VA greater than $1MM per portfolio. Note that individual rather than net IPV and VA balances should be reviewed as there may be offsetting effects within a portfolio.


References: 

[More details](ipv.md)


[Researchgate Guaranteed-Withdrawal-Notes](https://www.researchgate.net/profile/Tim-Xiao/publication/385743880_Pricing_Guaranteed_Withdrawal_Notes/links/6733981a69c07a4114454fdf/Pricing-Guaranteed-Withdrawal-Notes.pdf)




### All-In Gamma Shocks

Generate scenarios for the market instruments corresponding to the base and spread curves

Given the base and spread scenarios, those for the all-in curve can be generated and should be mapped according to spread name and contract date.  For instance, in the example above the AECOM: 201404 AllIn point would take absolute change from the AECOM: 201404 contract, and the base relative change and closing-rate from the NG: 201404

Using these scenarios, the absolute change for the all-in curve is constructed 


References: 

[More details](gammaShock.md)

[Researchgate zero](https://www.researchgate.net/profile/Tim-Xiao/publication/369920969_Zero_Curve_Construction/links/6434782bad9b6d17dc4b85f1/Zero-Curve-Construction.pdf)



### Commodity Risk Factor Translation

The goal of this work is to translate or convert simulated risk factors into market observables. There are three translations in commodity framework: price translation, volatility translation, and all-in translation.


References:

[More details](riskTranslation.md)

[Researchgate correlation swap](https://www.researchgate.net/profile/Tim-Xiao/publication/369898787_Correlation_Swap_Model/links/6431a73420f25554da1b4848/Correlation-Swap-Model.pdf)



### Commodity Volatility Closing Rate

We use the Omega type models to model the implied volatility skew for commodity derivatives.  These surfaces are incorporate moneyness and time to maturity into the skew definition and are a function of calibrated parameters (skew, wing, boost etc).


References:

[More details](volRate.md)

[Researchgate convertible](https://www.researchgate.net/profile/Tim-Xiao/publication/369881226_Convertible_Bond_with_Refix_Feature/links/643061d7609c170a13ff5527/Convertible-Bond-with-Refix-Feature.pdf)



### Precious Metal Futures Basis

Futures contracts are typically valued as a spread to the forwards curves.  This spread is the EFP (Exchange of Futures for Physical).  This function spec outlines the introduction of this spread as a basis risk factor into system and the transformation of sensitivities with respect to futures contracts to those with respect the spot contract, forward offered rates, and basis.

References:

[Researchgate binary](https://www.researchgate.net/profile/Tim-Xiao/publication/369878648_Binary_Return_Note_Model/links/64302aec20f25554da15a5ca/Binary-Return-Note-Model.pdf)



### Dividend Risk

OSFI recommended that dividend risk should be captured in market risk framework. To achieve that, a dividend risk model is developed by Market Risk (MR) and will be implemented in system. The model calls for the introduction of new dividend risk factors as the expected dividend amount of an equity asset, either a stock, or a basket of stocks, or an equity index. 


References:

[More details](dividend.md)

[Researchgate bet](https://www.researchgate.net/profile/Tim-Xiao/publication/369878537_Bet_Option_Model/links/643025894e83cd0e2f97a3b5/Bet-Option-Model.pdf)



### Dividend Exposure Measurement 

The proposal is to capture the dividend risk under normal market conditions. Stress test is considered a more appropriate approach to capture the risk of severe cutting or eliminating dividend of large blue chip stocks during financial crisis.


References:

[More details](divEx.md)

[Researchgate forward](https://www.researchgate.net/profile/Tim-Xiao/publication/369899083_Fixed_Forward_Option_Model/links/6431c9a9609c170a1302eb82/Fixed-Forward-Option-Model.pdf)



### Dividend Risk Modeling 

In practice, most traders treated dividend amount as “known” and risk managers do not monitor the price sensitivity to dividend amount as long as the total price sensitivity to underlying asset price is properly captured in case the dividend yield is used in pricing. If they think there is any dividend risk, that is only associated with the big negative jumps described above. Stress test, rather than daily VaR, is a proper way to capture that kind of risk.


References:

[More details](divModel.md)

[Researchgate cross](https://www.researchgate.net/profile/Tim-Xiao/publication/369997382_Cross_Currency_Swaption_Model/links/6438378620f25554da2bbae9/Cross-Currency-Swaption-Model.pdf)



### Dividend Risk Model Calibration

As described in model description and calibration of the model, the daily innovation to expected dividend of an index is simulated from double exponential distribution with specified correlation with all other risk factors. The daily innovation to expected dividend of a single stock is simulated on the fly without correlation with other risk factors. 


References:

[More details](divCalib.md)

[Researchgate dividend](https://www.researchgate.net/profile/Tim-Xiao/publication/369899100_Equity_Forward_with_Dividend_Reinvestment/links/6431d2e0609c170a1302ebe1/Equity-Forward-with-Dividend-Reinvestment.pdf)

