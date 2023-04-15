
### Early Start Swap Valuation

An early start swap is a swap that has an American style option for the counterparty of starting the swap early, within a period of three month. Otherwise, the swaps are plain vanilla fixed-for-floating swaps.

The swap start is the optimal time to enter the swap. Note also that the swap must start no later than the end day of the exercise period.

We consider a swap as an exchange of a principal for a coupon bearing bond with the same principal. Indeed, from payer’s perspective, the swap’s present value is the difference between the present values of received LIBOR payments

The term in the brackets can be considered as the value of a bond with a coupon c and a unit principal, while the first term in eq. (1) is the value of a zero coupon bond with a unit principal.

The present value of the swap is then calculated as the sum of present values of corresponding cash flows. To simulate the swap value at a later date, the coupon bond is represented through its forward rate of return. The internal rate of return at the valuation date is taken 

Further, we ignore the American feature of the option and treats it as European, with the earliest exercise date as the only exercise date. Effectively, the timing option is priced as an European option to exchange a swap at the end of the exercise period for one at the beginning of the period. 

The internal rates of return of the two swaps, one starting at the beginning and the other at the end of the exercise period, are generated for the earliest exercise date, assuming that the two rate are practically perfectly correlated. Then the difference of the present values of the two swaps, if positive, is taken as the option value. This value is averaged over a number of scenarios.

If the interest rates do not have random components, the difference in value between two swaps starting at different dates can be inferred from the present values of the corresponding cash flows, and then can be analytically calculated given the yield curve. The option value is then taken as the difference (if positive) between the maximal value of a swap starting within the exercise period and the value of the swap started at the beginning of the period. You can find more information on forward start option and cliquet option at https://finpricing.com/lib/EqCliquet.html

The relatively weak dependence of the option price on volatility suggests that the option price is dominated by its intrinsic value. This apparently is due to the facts that the length of period between the valuation date and the beginning of exercise interval, and especially the option tenor are small compared to the swap’s length., and that the internal rates of return for swaps starting at different dates are very strongly correlated

The analytical approach to the pricing of the option indicates that the modell should give the correct price as long as the present value of swap as a function of the effective date does not have a maximum, which exceeds the initial value, within the exercise interval.

Since the swap values are mostly affected by the yield of the longest maturity bond, this may occur when the yield curve has a noticeable hump after 10-year point for a period for about 3 month. Such a scenario seems quite unlikely and can hardly be detected on a conventional yield curve, whose points are normally one year (or more) apart.

References:

[ois pdf](https://osf.io/kapm3/download)

[zenodo base correlation approach pdf](https://zenodo.org/record/7831616/files/BaseCorrApproach.pdf)

[zenodo base correlation approach pdf](https://zenodo.org/record/7831616)

[zenodo base correlation test pdf](https://zenodo.org/record/7352694/files/baseCorrelationTest.pdf)

[zenodo base correlation test](https://zenodo.org/record/7352694)

