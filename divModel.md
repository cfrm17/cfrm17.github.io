
### Dividend Risk Modeling 


In practice, most traders treated dividend amount as “known” and risk managers do not monitor the price sensitivity to dividend amount as long as the total price sensitivity to underlying asset price is properly captured in case the dividend yield is used in pricing. If they think there is any dividend risk, that is only associated with the big negative jumps described above. Stress test, rather than daily VaR, is a proper way to capture that kind of risk.

We should bear in mind that the above view is only based on generic equity and equity derivative portfolios. As we can see, some derivative, such as long dated equity forwards and options, as well as dividend swaps, are very sensitive to expected dividend amount. Clearly, for these positions the dividend risk is no longer immaterial.

As we emphasized above (i.e. implied versus realized), the forward dividends instead of trailing dividends are used in yield calculation. 

Note that in financial mathematical term, the continuous dividend yield is defined as in the following equation:

Unlike bond coupon, the perceived dividend is not guaranteed. The market expectation of present value of total dividend to be received in a constant holding period may change day to day. This is due to the same reasons that drive the fluctuation of the market stock price. 


References:

[Hcommons creditVar](https://works.hcommons.org/records/ppetd-dfa44/files/creditvar.pdf?download=1)

[github touch](https://github.com/cfrm17/touchOption)

[github base](https://github.com/cfrm17/baseCorrelationModel)

[github arrpach](https://github.com/cfrm17/baseCorrelationApproach)
