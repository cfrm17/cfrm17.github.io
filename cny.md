
### CNY Curve Introduction


Valuation rate curves are foundations for FX derivative products. They serve two main purposes: the single curve can be used to discount future cash flows; and the pair curves can be used to estimate FX forward rates. 
The proposed CNY curve has two key instruments: SHIBOR Cash rate (short term up to 1 year) and SHIBOR 3 month swaps (long term up to 5 years). This proposed curve follows market practices. 

The CNY zero curve is generated using market quotes – SHIBOR rates up to 1 year and Bloomberg – interest rate swaps up to 5 years. For the USD FX curve the market quotes for the FX spot rates and FX forward spreads are 
taken from Reuters.

The model’s input components are: market quotes of underlying instruments, all parameter settings including business convention, day count, interpolation method, etc. Currently, curves are constructed using only SHIBOR 
Cash rates (R_d) and SHIBOR 3 month swaps (R_s).

The first two assumptions are market standard and hence acceptable. The third assumption is accepted considering most FX option deals are not beyond 5 years. Risk drivers are business conventions, valuation methodologies 
of the underlying instruments and the selected interpolation method. 

This approach is usually referred to as interest rate parity. This process assumes no arbitrage. That is, the returns from borrowing in one currency, exchanging that currency for another currency, and investing in the 
second currency while simultaneously purchasing futures to convert the currency back at the end of the holding period should be equal to the returns from purchasing and holding the first currency investment. If the returns 
differ, an arbitrage transaction could produce free money.


References:

[callable Asian option](https://ia902903.us.archive.org/31/items/callable-asian/CallableAsian.pdf)

[bond futures option](https://ia800506.us.archive.org/26/items/bond-futures-option/BondFuturesOption.pdf)

[Asian basket](https://ia903209.us.archive.org/22/items/asian-basket-rpo/AsianBasketRpo.pdf)





