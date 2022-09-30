
### Early Start Swap Valuation

An early start swap is a swap that has an American style option for the counterparty of starting the swap early, within a period of three month. Otherwise, the swaps are plain vanilla fixed-for-floating swaps.

The swap start is the optimal time to enter the swap. Note also that the swap must start no later than the end day of the exercise period.

We consider a swap as an exchange of a principal for a coupon bearing bond with the same principal. Indeed, from payer’s perspective, the swap’s present value is the difference between the present values of received LIBOR payments

The term in the brackets can be considered as the value of a bond with a coupon c and a unit principal, while the first term in eq. (1) is the value of a zero coupon bond with a unit principal.

The present value of the swap is then calculated as the sum of present values of corresponding cash flows. To simulate the swap value at a later date, the coupon bond is represented through its forward rate of return. The internal rate of return at the valuation date is taken 

Further, we ignore the American feature of the option and treats it as European, with the earliest exercise date as the only exercise date. Effectively, the timing option is priced as an European option to exchange a swap at the end of the exercise period for one at the beginning of the period. 

The internal rates of return of the two swaps, one starting at the beginning and the other at the end of the exercise period, are generated for the earliest exercise date, assuming that the two rate are practically perfectly correlated. Then the difference of the present values of the two swaps, if positive, is taken as the option value. This value is averaged over a number of scenarios.

If the interest rates do not have random components, the difference in value between two swaps starting at different dates can be inferred from the present values of the corresponding cash flows, and then can be analytically calculated given the yield curve. The option value is then taken as the difference (if positive) between the maximal value of a swap starting within the exercise period and the value of the swap started at the beginning of the period. You can find more information on forward start option and cliquet option at https://finpricing.com/lib/EqCliquet.html



References:

[pdf](https://osf.io/kapm3/download)

[list](https://osf.io/z587j/wiki/home/)





