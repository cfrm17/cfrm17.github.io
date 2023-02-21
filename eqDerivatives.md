## Equity Derivatives


### Asian Basket Options with Individually Capped Returns

We compute the payoff M times and then take the average. If M is large enough, then these average approaches the expectation we are looking for (an application of the Strong Law of Large Numbers). Alongside we also compute the statistical standard error. Note that if the valuation date is later than an averaging date, then on that date the realized price must be used in the computation of the payoffs. The sensitivities are computed using finite differencing with path recycling. 

References: 

[Zenodo Asian Basket pdf](https://zenodo.org/record/7474285/files/AsianBasket.pdf)

[Zenodo Asian Basket](https://zenodo.org/record/7474285)

[Github Asian Basket](https://github.com/cfrm17/asianBasket)
