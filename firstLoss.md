
### Giant First Loss Model


Compared to the standard first loss model with the same collateral pool and tranche structure, the new model predicts smaller B/E spreads for each tranche. Further, it is more sensible to the interest rate and the sensitivity to the interest rate term structure changes dramatically. The B/E spreads for each tranche calculated by both models converge when the hazard rates of the obligors become very small.


The new Giant First Loss model is a first loss trade structure in which all losses to the structure are held until the maturity of the trade. In this model, the amount of the principal for the tranches, upon which the coupons are paid, are fixed for the duration of the structure, rather than being modified as losses occur for the standard first loss model. The value of protection is calculated by solely using the discount factor at maturity of the trade, because all losses are settled at maturity.

Within the existing modeling framework, the trade is implemented by resetting generated default times in each Monte Carlo (MC) scenario to be the maturity date. Compared with the standard first loss trade model, two trends of change can be perceived. First, when the hazard rate of the obligor becomes smaller, the B/E spreads for both models would converge to zero. Second, because in the new model the cash flow pattern for default events has changed, the sensitivity to the interest rate should be different. Generally the new model is not only more sensitive to the interest rate but the sensitivity to its term structure changes dramatically as well. 

First, the sensitivity to the interest rate for the new model and the standard first loss model is compared. The results are shown in Table 2 with the detail results listed in Appendix II. Delta with 5bps parallel shift is calculated by giving a 5bps parallel up shift to the interest rate. Delta with 5bps tilt is computed by giving a 5bps tilt to the interest rate (clockwise tilt within 5 years).

We can find two trends. First, the new model is more sensitive. Given the same amount of perturbation to the interest rate, the change of present value (PV) for the new model is much larger than that of the standard model. Second, the sensitivity to term structure changes dramatically. For the standard first loss model, the Delta change between the parallel shift and the tilt is small while the change is very large for the new model. 



References:

[credit risk](https://figshare.com/articles/preprint/_b_The_Impact_of_Collateralization_on_Derivatives_Markets_b_/24201222)

[credit risk pdf](https://figshare.com/articles/preprint/_b_The_Impact_of_Collateralization_on_Derivatives_Markets_b_/24201222/2/files/42470781.pdf)





