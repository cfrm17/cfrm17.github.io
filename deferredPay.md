
### Deferred CDO Coupon Payment 


The deferred CDO coupon payment valuation model serves the purpose of valuing the accumulated coupon payments held in a non-interest-bearing reserve account for a CDO trade.  It is a part of the valuation model for a non-vanilla CDO structure called “rated equity.”

The model is a straightforward extension of the existing valuation model for vanilla CDO trades. The amount of each deferred coupon payment is calculated the same way as a vanilla CDO trade. Because the reserve account is non-interest-bearing, all the cash flows held in the account are discounted using the discount factor at the trade maturity. Note that for an interest-bearing reserve account, accumulated coupon payments are valued in the same as a vanilla CDO trade case and no new model is required.

The model serves the purpose of computing the value of the accumulated coupon payments held in the non-interest-bearing reserve account for a CDO trade [1]. It is a part of the valuation model for a non-vanilla CDO trade called “rated equity”, which is defined as an equity tranche with part of its coupon payments held in a reserve account. 

Modeling the accumulated coupon payments is straightforward within the current structured credit derivative modeling framework. The amount of each coupon payment is calculated the same way as a vanilla CDO trade. Because the reserve account is non-interest-bearing, all the cash flows held in the account are discounted using an appropriate discount factor at the trade maturity. Note that for an interest bearing reserve account, accumulated coupon payments are valued in the same way as that for a vanilla CDO trade and no new model is required.

The model is different from a vanilla CDO model in terms of the treatment of discounting. The model is straightforward and it not necessary to test against other benchmark models.

Two series of testing were designed to investigate the model. First, the submitted model was tested by an independent implementation of the model via existing approved models for vanilla CDO trades in the Oscar-Fritz library. By manipulating the discount factor, we replicated the value of the accumulated coupon payments without-interest-bearing using a vanilla CDO model. Assuming a zero discount factor, we calculated the accumulated coupon payments using the vanilla CDO model. The value of the reserve account was then computed by discounting these fee payments with discount factor at trade maturity. 


References:

[zenodo pdf](https://zenodo.org/record/7374179/files/DeferredPay.pdf)

[archive extendable Swap](https://ia601509.us.archive.org/6/items/extendableSwap/extendableSwap.pdf)

[gitbook cash](https://finwhite.gitbook.io/arbitrarycash/)

[github forward](https://github.com/cfrm17/specialEquityForward)

[osf var](https://osf.io/uzpk3/download)
