
### Ratchet Swap Valuation

A ratchet swap is an interest rate swap with two legs. One leg is a standard floating leg and the other leg is a ratchet leg. The ratchet leg pays a ratchet floating rate.

The ratchet floating rate coupon is based on an index, e.g., 6-month EURIBOR. The rate is further subject to a minimum decrease of 0 bps and a maximum increase of a threshold, such as, 15 bps. These rates are reset two business days prior to the first day of each coupon period. 

We denote these payments dates, which are 0.5 years apart under 30/360 and are subject to modified business day conventions

The coupon rate is stated as an annualized rate or real rate based on market conventions. Adjustment is made for long/short first/last coupon periods. When a coupon date falls on non-business day, payment may be made next business day with no amount adjustment, see https://finpricing.com/lib/FiBondCoupon.html

The valuation methodology is based on the Monte Carlo spot LIBOR rate model. The model generates spot rates which log-normally distributed at each reset date. These spot rates are derived from corresponding forward rates whose stochastic behavior is constructed in an arbitrage-free manner. Outcomes for the spot rate are generated for each reset date. These rates are then applied to the ratchet-type payoff structure. The ratchet instrument is then valued by discounting and averaging these payoffs.

The valuation is based on the Monte Carlo spot LIBOR rate model. The model generates spot rates which log-normally distributed at each reset date. These spot rates are derived from corresponding forward rates whose stochastic behavior is constructed in an arbitrage-free manner.

References:

[pdf](https://osf.io/azy78/download)

[list](https://finpricing.com/FinPricing-ProductBrochure.pdf)





