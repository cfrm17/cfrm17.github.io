## Risk Management


One of the central tenets of financial economics is the necessity of some trade off between risk and expected return. Because high risk is associated 
with high reward, investor may potentially obtain higher profits only if he is willing to accept a higher chance of losses. Risk-return trade-off is 
one trading principal in financial markets.

Risk management is a process to identify and measure risk. The goal of risk management solution is to ensure that risk is under limit and there is no 
surprise in future. In capital markets, risk management is accountable for oversighting and monitoring the profit and loss, market risk, credit risk, 
liquidity risk and valuation risk activities of a firm.

Capital market risk management system is an information technology platform that helps people in financial markets balance risk appetite with performance 
to ultimately optimize capital efficiency, identify probblems, mitigate threats, control risk, avoid unexpected loss, and enhance opportunities.

Market risk is the risk of losses in positions due to market movements, whereas counterparty credit risk refers to the risk that a counterparty to 
a bilateral financial derivative contract may fail to fulfill its contractual obligation causing financial loss to the non-defaulting party. FinPricing 
offers capital market risk management products and services to help your organization effectively identify and address the risk you face in financial 
markets.

### Counterparty Credit Risk

Counterparty credit risk measurement is credit exposure (CE). It is the cost of replacing or hedging a contract at the time of default. Other measures 
include Potential future exposure (PFE), Expected exposure (EE), Expected Positive Exposure (EPE), Effective expected exposure (EEE), Effective EPE, 
Exposure at default or EAD. 

[Counterparty Credit Risk](ccr.md)

[OSF ccr](https://osf.io/2dg48/download)

[Archive ccr](https://ia600105.us.archive.org/18/items/alex_Ccr/ccr-1.pdf)

[OSF pooling](https://osf.io/atyb9/download)


### Credit Risk Simulation

o calculate credit exposure or replacement cost in future times, one needs to simulate market evolutions. Simulation must be conducted under the 
real-world measure. One could use a simple but inaccurate solution, or accurate but complex approach. Some vendors and institutions use this simplified 
approach. Only a couple of stochastic processes are used to simulate all market risk factors. They use Vasicek model for all mean reverting factors
dr=k(θ-r)dt+σdW where r – risk factor; k – drift; θ – mean reverse; σ – volatility; W – Wiener process. And use Geometric Brownian Motion (GBM) for all 
non-mean reverting risk factors: dS=μSdt+σSdW. The calibration results for different risk factors are different from each other.

[Counterparty Credit Risk Monte Carlo Simulation](ccrsimulation.md)

[OSF ccr sim](https://osf.io/s5b4u/download)

[Archive ccr sim](https://ia801006.us.archive.org/24/items/ccrSimulation/ccrSimulation-2.pdf)

[FlipHtml5 ccr sim](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamkDN4UzM5ITPkl0av9mY)

[OSF himalaya](https://osf.io/cg5x4/download)




### Collateral Management

In the derivatives world, collateral posting is a risk reduction tool that mitigates risk by reducing credit exposure. It allows financial institutions 
to reduce economic capital and credit risk, free up lines of credit, and expand the range of counterparties. All of these factors contribute to the 
growth of financial markets. The benefits are broadly acknowledged and affect dealers and end users, as well as the financial system generally.  


[Collateral Management](collateral.md)

[OSF collateral](https://osf.io/zuhcw/download)

[Archive collateral](https://ia803105.us.archive.org/8/items/collateral_201804/collateral-3.pdf)

[Science Media collateral](http://science-media.org/userfiles/1020/presentations/1020_presentation_434.pdf)

[FlipHtml5 collateral](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamATN4UzM5ITPkl0av9mY)

[OSF securization](https://osf.io/vzfaw/download)



### CVA

CVA, by definition, is the difference between the risk-free portfolio value and the true (or risky or defaultable) portfolio value that takes into 
account the possibility of a counterparty’s default. The risk-free portfolio value is what brokers quote or what trading systems or models normally 
report. The risky portfolio value, however, is a relatively less explored and less transparent area, which is the main challenge and core theme for CVA. 
In other words, central to CVA is risky valuation.


[Credit Valuation Adjustment](cva.md)

[OSF cva](https://osf.io/hygf7/download)

[Zenodo cva](https://zenodo.org/record/4016321/files/cva-4.pdf)

[FlipHtml5 cva](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamAjMwkzM5ITPkl0av9mY)

[Archive cva](https://ia801000.us.archive.org/32/items/alex_Cva_201804/cva-4.pdf)

[OSF Brownian](https://osf.io/6dn54/download)




### FVA

FVA is the cost of funding that is considered in the valuation of uncollateralized derivatives. It is introduced to quantify the adjustment to the 
value of derivatives in order to ensure that a trader recovers funding costs that are consistent with the market’s view of the funding costs associated 
with the same trade. This presentation elaborates an integrated framework for calculating both CVA and FVA. We also discuss the pros and cons of comparing 
the popular credit exposure approach and the more accurate least square Monte Carlo approach. 


[Funding Valuation Adjustment](fva.md)

[OSF fva](https://osf.io/r6y2h/download)

[Archive fva](https://ia801009.us.archive.org/21/items/cvaFva/cvaFva-5.pdf)

[Science Media fva](https://science-media.org/userfiles/1020/presentations/1020_presentation_466.pdf)

[FlipHtml5 fva](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamIzMwkzM5ITPkl0av9mY)

[OSF gic](https://osf.io/tgd82/download)




### FRTB

FRTB provides a clear definition of the boundary between the trading book and the banking book. It consists of an overhaul of the internal model 
approach (IMA) to focus on tail risk and an overhaul of the standardized approach (SA) to make it more risk sensitive. Each approach also explicitly 
captures default risk and other residual risks. Liquidity risk is explicitly included for different asset classes via liquidity horizons.


[FRTB Standarlized Approach](frtb.md)

[OSF frtb](https://osf.io/pn768/download)

[Archive frtb](https://ia601407.us.archive.org/28/items/frtbSa-6/frtbSa-6.pdf)

[Science Media frtb](https://science-media.org/userfiles/1020/presentations/1020_presentation_467.pdf)

[FlipHtml5 frtb](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamMDNwkzM5ITPkl0av9mY)

[OSF local vol](https://osf.io/74s83/downloand)




### Historical VaR

The historical VaR approach follows the following procedures: First, obtain one year historical value time series of all market factors, such as a stock 
price time series is ■(x ̅_1&⋯&x ̅_251 ). Assuming today’s value is x_0, generate 250 historical scenarios. The i-th is  x_i=(x ̅_i⁄x ̅_(i-1) -1)x_0. 
Compute base PV at today t as P(x_o), Compute 250 scenario PVs:  P(x_i). Then derive 250 scenario P&L:	P(x_i )-P(x_0). Finally sort 250 scenario P&L. 
The VaR is the average between 2nd and 3rd lowest (negative) numbers.


[Historical Value at Risk](historicalVaR.md)

[OSF var](https://osf.io/m9j7v/download)

[Archive var](https://ia801502.us.archive.org/15/items/historical-va-r-7/HistoricalVaR-7.pdf)

[Zenodo var](https://zenodo.org/record/4017733/files/HistoricalVaR-7.pdf)

[Science Media var](https://science-media.org/userfiles/1020/presentations/1020_presentation_468.pdf)

[FlipHtml5 var](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamQDO1UDN5ITPkl0av9mY)

[OSF asset back](https://osf.io/eg6mv/download)




### SIMM

Initial margin calculation is counterparty-portfolio-based. It applies to non-cleared OTC derivatives only. Derivative trades belonging to a counterparty 
will be divided into cleared-trade portfolio and non-cleared-trade portfolio. The initial margin is computed for the non-cleared portfolio. 

Margin is collateral that one party needs to deposit with a broker or an exchange to cover some or all of market risk or credit risk. There are several types
of margin. Initial Margin is the amount of collateral required to open a position. Maintenance Margin is the minimum amount of collateral required to 
keep the position open after inception. If (Margin balance) < (Maintenance margin), the broker issues a margin call that requires the investor to bring 
the margin balance back to initial margin.


[Standard Initial Margin Model](simm.md)

[OSF simm](https://osf.io/ybfuz/download)

[Archive simm](https://ia801501.us.archive.org/28/items/initialMargin-8/initialMargin-8.pdf)

[Zenodo simm](https://zenodo.org/record/4025373/files/initialMargin-8.pdf)

[FlipHtml5 simm](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamYTO1UDN5ITPkl0av9mY)

[OSF bond curve](https://osf.io/4nhyb/download)



### IRC

To caluclate IRC, one needs to simulate default and migration for one-year horizon. Also, one needs to take concentration into account, that measures 
the degree of a portfolio diversification. For example, if a significant number of issuers belong to a certain category, the portfolio is a concentrated 
one.


[Incremental Risk Charge](irc.md)

[OSF irc](https://osf.io/4fdjm/download)

[Archive irc](https://ia601401.us.archive.org/13/items/irc-9/irc-9.pdf)

[Zenodo irc](https://zenodo.org/record/4025375/files/irc-9.pdf)

[Science Media irc](https://science-media.org/userfiles/1020/presentations/1020_presentation_471.pdf)

[FlipHtml5 irc](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamEDM2UDN5ITPkl0av9mY)

[OSF hw vol](https://osf.io/k3wc9/download)




### Market

One of the central tenets of financial economics is the necessity of some trade off between risk and expected return. This presentation gives an overview 
of financial market basics. Click the links below for details. People in financial market care about returns. Financial return is the measure of profit or 
loss on an investment. Return is more important than value itself.

[Financial Market](market.md)

[OSF market](https://osf.io/rbxqz/download)

[Archive market](https://ia801000.us.archive.org/29/items/market_20180417/market-10.pdf)

[Zenodo market](https://zenodo.org/record/4025380/files/market-10.pdf)

[Science Media market](https://science-media.org/userfiles/1020/presentations/1020_presentation_472.pdf)

[FlipHtml5 market](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamcDM2UDN5ITPkl0av9mY)

[OSF exchangeable](https://osf.io/zgx8c/download)




### Economic Capital

Economic capital falls into the category of Value at Risk (VaR) measures as both try to capture value change due to market movement. Most institutions use the 
existing VaR system to compute economic capital. VaR captures the market risk of 1-day time period at 99% confidence level whereas Economic capital measures the 
market risk of 1-year time period at 99.95 confidence level. Therefore, scaling methodology is the key to compute economic capital, i.e., scaling 1-day to 1-year 
and 99% to 99.95%. This presentation is intended to answer several fundamental economic capital questions: what is economic capital? What is the difference 
between economic capital and regulatory capital? How to compute economic capital? 


[Market Risk Economic Capital](mrEc.md)

[OSF capital](https://osf.io/fdmb4/download)

[Archive capital](https://ia803108.us.archive.org/21/items/alex_MrEc/mrEc-11.pdf)

[Zenodo capital](https://zenodo.org/record/4027801/files/mrEc-11.pdf)

[Science media capital](https://science-media.org/userfiles/1020/presentations/1020_presentation_473.pdf)

[FlipHtml5 capital](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamYTNzQTN5ITPkl0av9mY)

[OSF forward starting](https://osf.io/37fbt/download)




### Parametric VaR

Value at Risk (VaR) is the regulatory measurement for assessing market risk. It reports the maximum likely loss on a portfolio for a given probability defined 
as x% confidence level over N days. VaR is vital in market risk management and control. Also regulatory and economic capital computation is based on VaR results. 
Although VaR measure is objective and intuitive, it doesn’t capture tail risk. There are three commonly used methodologies to calculate VaR – parametric, 
historical simulation and Monte Carlo simulation. This presentation focuses on parametric VaR.  


[Parametric Value at Risk](parametricVaR.md)

[OSF Par VaR](https://osf.io/uzpk3/download)

[Archive Par VaR](https://ia801502.us.archive.org/29/items/parametric-va-r-12/ParametricVaR-12.pdf)

[Science media Par VaR](https://science-media.org/userfiles/1020/presentations/1020_presentation_474.pdf)

[FlipHtml5 Par VaR](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamUjNzQTN5ITPkl0av9mY)

[OSF 3 factors](https://osf.io/pbjf8/download)



### Sensitivity

Risk sensitivities or Greeks are vital for risk management. They can help financial market participants isolating risk, hedging risk and explaining profit & loss. 
This presentation gives certain practical insights onto this topic. 

Delta is a first-order Greek that measures the value change of a financial instrument with respect to changes in the underlying asset price. Vega is a first-order 
Greek that measures the value change of a financial instrument with respect to changes in the underlying implied volatility. Gamma is a second order Greek that 
measures the value change of a financial instrument with respect to changes in the underlying price. Theta is a first order Greek that measures the value change 
of a financial instrument with respect to time.


[Financial Sensitivity](sensitivity.md)

[OSF sensitivity](https://osf.io/qau3b/download)

[Archive sensitivity](https://ia903107.us.archive.org/18/items/sensitivity_201804/sensitivity-13.pdf)

[Science Media sensitivity](https://science-media.org/userfiles/1020/presentations/1020_presentation_475.pdf)

[FlipHtml5 sensitivity](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamcjNzQTN5ITPkl0av9mY)

[OSF hw convertible](https://osf.io/eyb8c/download)



### Monte Carlo VaR

Monte Carlo VaR assumes  market factors follow certain stochastic processes. It has easy back and stress test and is good for high confidence level and 
tail risk. The drawbacks are dependent on distribution assumption and calibration is required. Most importantly it requires extensive computation.

The only way to verify a VaR system is backtest. At a certain day, compute hypothetic P&L (valuation date and portfolio unchanged). If (hypothetic P&L > VaR), 
then breaches. For one year, if number of breaches is 0-4, the VaR system is in Green zone. If number of breaches is 5-9, the VaR system is in Yellow zone
If number of breaches is 10 or more, the VaR system is in Red zone.

[Monte Carlo Value at Risk](mcVaR.md)

[OSF mc var](https://osf.io/2a58h/download)

[Archive mc var](https://ia801407.us.archive.org/30/items/monte-carlo-va-r-14/MonteCarloVaR-14.pdf)

[Science Media mc var](https://science-media.org/userfiles/1020/presentations/1020_presentation_476.pdf)



[Independent Valuation](independentValuation.md)
