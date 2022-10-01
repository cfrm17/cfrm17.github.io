
### Digital Swap Valuation

A daily digital LIBOR swap is an interest rate swap whose reference interest rate is three-month USD Libor BBA. For each accrual period in the swap, one party receives the reference rate, and pays the reference rate plus a positive spread, but weighted by the ratio of the number of calendar days in the period that the reference rate sets below an upper level to the total number of calendar days in the period.

The payoff amount can be viewed as the value of the sum of a series of daily Libor digital payoffs.  Here we assume that Libor rates are log-normally distributed, and derives an analytical formula for the daily digital payoff.

Consider a particular accrual period.  With respect to this period, let 

•	  denote the reference rate reset time (expressed in years),

•	  be the spot reference rate at the reset time,

•	  denote the period’s  interval of time (in years).

Then, at time  T, Northern Rock PLC pays the reference rate times the accrual period’s interval of time,

The payoff amount can be viewed as the value of the sum of a series of daily Libor digital payoffs. Here we assume that Libor rates are log-normally distributed, and derives an analytical formula for the daily digital payoff.

We assume that Libor rates follow geometric Brownian motion with no drift and constant volatility under their respective forward measures. In order to value a daily Libor-based digital payoff, the respective Libor rates at the daily setting time and at the accrual period start must then be expressed under the same forward measure.

We apply respective convexity and timing delay adjustments to the daily Libor’s forward value. The payoff is then priced based on an analytical formula that involves cumulative normal distribution terms. We note that the distributional assumptions for the bonds underlying the convexity and timing delay adjustments can be refined, however, if more pricing accuracy is required.

We have tested the swap’s daily Libor-based digital pricing over two accrual periods, respectively, starting in 0.4 years and 2.45 years. We also stress tested the WM daily digital pricing for an accrual period beginning in approximately 9.5 years. We find that the model is very accurate.

References:

[pdf](https://osf.io/qzmer/download)

[list](https://osf.io/wn2ys/wiki/home/)





