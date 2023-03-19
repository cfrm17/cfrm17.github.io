
### Standardized Initial Margin Model

Initial Margin (IM) is the amount of collateral required to open a position with a broker or an exchange or a bank. The Standard Initial Margin Model (SIMM) 
is very likely to become the market standard. It is designed to provide a common methodology for calculating initial margin for uncleared OTC derivatives. 
Initial margin calculation is counterparty-portfolio-based. Given this standardized approach, counterparties can easily reconcile the results. 

Initial margin calculation is counterparty-portfolio-based. It applies to non-cleared OTC derivatives only. Derivative trades belonging to a counterparty 
will be divided into cleared-trade portfolio and non-cleared-trade portfolio. The initial margin is computed for the non-cleared portfolio. 

Margin is collateral that one party needs to deposit with a broker or an exchange to cover some or all of market risk or credit risk. There are several types
of margin. Initial Margin is the amount of collateral required to open a position. Maintenance Margin is the minimum amount of collateral required to 
keep the position open after inception. If (Margin balance) < (Maintenance margin), the broker issues a margin call that requires the investor to bring 
the margin balance back to initial margin.

SIMM calculation is conducted from the lowest level to the highest one: first define risk factors; second, aggregate risk into risk buckets; third, add risk
at risk easures; fouth, futher aggregate risk at risk classes and then products classes. Finally compute the total initial margin.

From the top, there are four product classes: Interest Rates and Foreign Exchange (RatesFX), Credit, Equity, and Commodity.

There are a total of six risk classes: Interest Rate, Credit (Qualifying) with non-securitization and simple securitization, Credit (Non-Qualifying)
with complex securitization, Equity, Commodity, and FX.

It defines three risk measures: Delta, Vega, and Curvature. It further defines risk buckets for each risk class.


Reference: 

[SIMM](/initialMargin-8.pdf)

[Zenodo simm](https://zenodo.org/record/4025373/files/initialMargin-8.pdf)

[Fliphtml5 simm](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamYTO1UDN5ITPkl0av9mY)

[OSF tree](https://osf.io/6eyrv/download)

[OSF martingale tree](https://osf.io/6eyrv/download)

[OSF simm](https://osf.io/ybfuz/download)

[OSF bond curve](https://osf.io/4nhyb/download)
