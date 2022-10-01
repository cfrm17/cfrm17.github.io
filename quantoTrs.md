
### Quanto Total Return Swap Valuation

A quanto total return Libor Swap is a swap where one leg is a regular floating leg paying LIBOR less a constant spread and the other leg makes a single payment at the swap’s maturity equal to a leveraged non-negative return on USD-for-EURO exchange rate paid in CAD. The main focus of the valuation model is the quantoed total return on the FX rate.

The payoff of the leg based on the return of the foreign exchange rate is a payoff of a European call option.  Its present value is given by Black’s formula for futures with the discounting factor equal to the Canadian zero-coupon bond and the future price 

The important point is that the option price depends on the volatilities and correlation of the exchange rates as well as on the interest rates of all the three currencies.

Let XUE(t) be the USD-for-EURO exchange rate at time t, which gives the amount of USD funds exchanged for one EURO. Let XUC(t) be a similar USD-for-CAD exchange rate. Assume further that both rates follow geometric Brownian motions with constant volatilities under the natural probability measure

Since the valuation of the floating leg is straightforward, the main challenge is the valuation of the quanto-return based leg.

The present value of the floating leg can be calculated as the price of a swap whose one leg pays LIBOR and the other pays the negative spread.

The payoff of the quanto-return leg is max(1.3 x (FX at maturity - initialFX)/initialFx), 0). In other words, The payoff of the leg based on the return of the foreign exchange rate is a payoff of a European call option. Its present value is given by Black’s formula for futures with the discounting factor equal to the Canadian zero-coupon bond and the future price.

The tests were focused on intrinsic, typical and extreme cases:

• deterministic case – volatility of the USD-for-EURO exchange rate 0.1%;

• typical case – volatility of the USD-for-EURO exchange rate 13.4%;

• extreme case – volatility of the USD-for-EURO exchange rate 90%.

References:

[pdf](https://osf.io/p7kn4/download)

[list](https://osf.io/rwfgn/wiki/home/)





