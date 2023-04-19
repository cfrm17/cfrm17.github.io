
### FX Option Valuation via BGM

The interest rate diffusion refers to the Brace-Gatarek-Musiela (BGM) model that is a multi-factor log-normal model. The very brief description of BGM approach in Monte Carlo setting is

	Select almost periodic grid of forward dates, typically 3m apart

	Select arbitrary grid of diffusion dates based on reset dates of exotic security which user aims to price

	Postulate that simple rates between any two consecutive forward dates, as observed on any diffusion date, are distributed lognormally (as well as simple rate between observation date and first forward date greater than it)

	Determine parameters of the lognormal distributions of the forward rates: 

If the maturity falls in between two consecutive diffusion dates, then a partial diffusion from the last diffusion date before maturity to the exact maturity date is performed.

In order to increase accuracy, we observe that, on the last step, the volatility and the interest rates do not vary anymore. Hence, the option can be computed by Black-Scholes formula. This will smooth the pay-off and fasten the convergence. For intermediate maturities, this technique also avoids partial diffusion.

For knock-out options, the sum is only performed on those trajectories that do not hit the barrier(s), although we still divide it by the total number  . However, especially when computing sensitivities, a discontinuity may occur if a path reaches a point very close to the barrier without crossing it, and finishes in the money.

To avoid such problems, trajectories are weighted according to their survival probability. One can imagine each trajectory as representing a whole beam of paths, of which we only know their values at the observation dates, but that can “wander” in between these dates. Thus, some of them may be killed because they hit the barrier between observation dates. By a “Brownian bridge” technique, the proportion of those who hit the barrier for each trajectory and in each interval  is computed


References:

[archive pdf](https://ia904708.us.archive.org/21/items/fxOptionBGM/fxOptionBGM.pdf)

[gitbook bgm](https://finwhite.gitbook.io/mcbgm/)

[github tree](https://github.com/timxiao1203/MartingalePreservingTree)

[core credit pdf](https://core.ac.uk/download/222936038.pdf)

[core credit](https://core.ac.uk/works/64801172)

