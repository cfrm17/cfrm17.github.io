## Financial Academics




### Credit Valuation Adjustement and Wrong Way Risk


CVA not only allows institutions to move beyond the traditional control mindset of credit risk limits and to quantify counterparty risk as a single measurable P&L number, but also offers an opportunity for banks to dynamically manage, price and hedge counterparty risk. 

CVA, by definition, is the difference between the risk-free portfolio value and the true (or risky or defaultable) portfolio value that takes into account the possibility of a counterparty’s default. The risk-free portfolio value is what brokers quote or what trading systems or models normally report. The risky portfolio value, however, is a relatively less explored and less transparent area, which is the main challenge and core theme for CVA. 


References:

[Core cva](https://core.ac.uk/download/328766597.pdf)





### LIBOR Market Model Implementation

The LIBOR Market Model has become one of the most popular models for pricing interest rate products. It is commonly believed that Monte-Carlo simulation is the only viable method available for the LIBOR Market Model. In this article, however, we propose a lattice approach to price interest rate products within the LIBOR Market Model by introducing a shifted forward measure and several novel fast drift approximation methods. This model should achieve the best performance without losing much accuracy. Moreover, the calibration is almost automatic and it is simple and easy to implement. Adding this model to the valuation toolkit is actually quite useful; especially for risk management or in the case there is a need for a quick turnaround.


References:

[More](McBgm.md)

[Core lmm pdf](https://core.ac.uk/download/288179622.pdf)

[Core lmm](https://core.ac.uk/works/10287558)




### Pricing Convertible Bond

This paper presents a new model for valuing hybrid defaultable financial instruments, such as, convertible bonds. In contrast to previous studies, the model relies on the probability distribution of a default jump rather than the default jump itself, as the default jump is usually inaccessible. As such, the model can back out the market prices of convertible bonds. A prevailing belief in the market is that convertible arbitrage is mainly due to convertible underpricing. Empirically, however, we do not find evidence supporting the underpricing hypothesis. Instead, we find that convertibles have relatively large positive gammas. As a typical convertible arbitrage strategy employs delta-neutral hedging, a large positive gamma can make the portfolio highly profitable, especially for a large movement in the underlying stock price.


References:

[Core convertible pdf](https://core.ac.uk/download/214006918.pdf)

[Core convertible](https://core.ac.uk/works/8874494)




### Bilateral Credit Risk

The one-side defaultable financial derivatives valuation problems have been studied extensively, but the valuation of bilateral derivatives with asymmetric credit qualities is still lacking convincing mechanism. This paper presents an analytical model for valuing derivatives subject to default by both counterparties. The default-free interest rates are modeled by the Market Models, while the default time is modeled by the reduced-form model as the first jump of a time-inhomogeneous Poisson process. All quantities modeled are market-observable. The closed-form solution gives us a better understanding of the impact of the credit asymmetry on swap value, credit value adjustment, swap rate and swap spread.


References:

[Core bilateral pdf](https://core.ac.uk/download/534863091.pdf)

[Core bilateral](https://core.ac.uk/works/125992166)




### Jump Diffusion Model

This paper argues that the reduced-form jump diffusion model may not be appropriate for credit risk modeling. To correctly value hybrid defaultable financial instruments, e.g., convertible bonds, we present a new framework that relies on the probability distribution of a default jump rather than the default jump itself, as the default jump is usually inaccessible. As such, the model can back out the market prices of convertible bonds. A prevailing belief in the market is that convertible arbitrage is mainly due to convertible underpricing. Empirically, however, we do not find evidence supporting the underpricing hypothesis. Instead, we find that convertibles have relatively large positive gammas. As a typical convertible arbitrage strategy employs delta-neutral hedging, a large positive gamma can make the portfolio highly profitable, especially for a large movement in the underlying stock price.


References:

[Core jump pdf](https://core.ac.uk/download/534862401.pdf)

[Core jump](https://core.ac.uk/works/127927866)



### Credit Risk

This article presents a new model for valuing financial contracts subject to credit risk and collateralization. Examples include the valuation of a credit default swap (CDS) contract that is affected by the trilateral credit risk of the buyer, seller and reference entity. We show that default dependency has a significant impact on asset pricing. In fact, correlated default risk is one of the most pervasive threats in financial markets. We also show that a fully collateralized CDS is not equivalent to a risk-free one. In other words, full collateralization cannot eliminate counterparty risk completely in the CDS market.


References:

[Core credit risk pdf](https://core.ac.uk/reader/334593150)

[Core credit risk](https://core.ac.uk/works/8882406)




### IRC

The incremental risk charge (IRC) is a new regulatory requirement from the Basel Committee in response to the recent financial crisis. Notably few models for IRC have been developed in the literature. This paper proposes a methodology consisting of two Monte Carlo simulations. The first Monte Carlo simulation simulates default, migration, and concentration in an integrated way. Combining with full re-valuation, the loss distribution at the first liquidity horizon for a subportfolio can be generated. The second Monte Carlo simulation is the random draws based on the constant level of risk assumption. It convolutes the copies of the single loss distribution to produce one year loss distribution. The aggregation of different subportfolios with different liquidity horizons is addressed. Moreover, the methodology for equity is also included, even though it is optional in IRC.


References:

[Core irc pdf](https://core.ac.uk/download/334593149.pdf)

[Core irc](https://core.ac.uk/works/8882346)



### CDS

This article presents a new model for valuing a credit default swap (CDS) contract that is affected by multiple credit risks of the buyer, seller and reference entity. We show that default dependency has a significant impact on asset pricing. In fact, correlated default risk is one of the most pervasive threats in financial markets. We also show that a fully collateralized CDS is not equivalent to a risk-free one. In other words, full collateralization cannot eliminate counterparty risk completely in the CDS market.


References:

[Core cds](https://core.ac.uk/download/534863097.pdf)



### Commodity Factor Model

The random component of commodity future prices can be generally broken down into major contributors or factors. These are known as principal components. In this paper, we present a multi-factor framework for modeling commodity price dynamics. We develop a generic procedure for the model calibration. The calibration procedure consists of an offline step and an online step. Empirical and numeric study shows that the model prices fluctuate randomly around the market prices, indicating prima facie that the model performs quite well. 


References:

[Core commodity pdf](https://core.ac.uk/download/533453681.pdf)

[Core commodity](https://core.ac.uk/works/124575278)



### Local Vol Greek 

Calculation of the Greeks in the local volatility model is difficult because recalibrating the local volatility surface tends to result in high numerical error terms. While this appears to be OK for first order Greeks, for higher order Greeks we are forced to make some approximations. 


References:

[Detals](volGreek.md)



### Variable Rate MBS

The Canada Housing Trust (“CHT”) will raise funds by issuing Canada Mortgage Bonds and use the proceeds to purchase VRMBS’s from Approved Sellers. For each VRMBS purchased CHT will also enter into a swap, where it pays the MBS interest and reinvestment income to the swap counterparty and receives fixed coupon cashflows, which are used to service the CMB. CHT will also pay CMHC an up-front guarantee fee for each CMB issuance. In return CMHC provides a guarantee for the CMB’s.


References:

[Detals](variableMbs.md)



### Giant First Loss 

Compared to the standard first loss model with the same collateral pool and tranche structure, the new model predicts smaller B/E spreads for each tranche. Further, it is more sensible to the interest rate and the sensitivity to the interest rate term structure changes dramatically. The B/E spreads for each tranche calculated by both models converge when the hazard rates of the obligors become very small.


References:

[Detals](firstLoss.md)




### Forward Starting CDO 

Compared to the standard first loss model with the same collateral pool and tranche structure, the new model predicts smaller B/E spreads for each tranche. Further, it is more sensible to the interest rate and the sensitivity to the interest rate term structure changes dramatically. The B/E spreads for each tranche calculated by both models converge when the hazard rates of the obligors become very small.


References:

[Detals](firstLoss.md)



### Ratio Tunnel Option 

A ratio tunnel option offers the contract holder the right either long or short, at a contract maturity, a preset underlying collar. Notional principals and strikes in the collar may be different. In the system, the ratio tunnel option and the underlying collar are strictly European type. The ratio tunnel option model applies analytical close form pricing formulae for vanilla compound options.

References:

[Detals](ratioTunnel.md)


### Hedge Fund Return 

Daily net asset value of hedge funds normally are not market observable. The model allows financial market participants to produce a daily mark-to-model for their hedge fund positions, and eventually options derived thereon. We use the historical data of indices to generate a robust estimate of the required index weighting parameters. Empirical study shows that the model makes reasonable predictions when appropriate index choices have been made and produces diagnostic information that can indicate the relative reliability of predicted daily hedge fund returns.

References:

[Detals](hedgeFundReturn.md)


### Bond Option

The Pricer Bond Option (European style) assumes that the forward bond price is lognormal with a constant volatility. We use an analytical solution based on Black’s model for European options.

[Detals](bondOption.md)

