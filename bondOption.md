
### Bond Option


According to an ISDA agreement we see that when a bond option is exercised, the holder pays the strike price (which is a clean price) plus accrued. The accrued component of the dirty price is deterministic, so it is 
not a very interesting quantity from the perspective of pricing an option. Think of it this way, say one exercise a call on a bond and pay the strike (clean) plus accrued for regular settlement. We can simultaneously 
sell the bond in the open market and we will get the market clean price plus the same accrued, so the accrued in effect cancel out. Therefore, we suggest that the clean price in the Black’s model.

NDelta is change in NPV induced by 1 basis point shift in the zero curve(s). We move the whole curve of zero rates simultaneously up by 1 basis point, re-price and give back the change in NPV.

NGamma is change in NDelta induced by the shift of the zero curve(s) 1 basis point up. We move the whole curve of zero rates simultaneously up by 1 basis point, re-price and give back the change in NPV.

NVega is numerical approximation of Vega. We move the whole volatility surface of the underlying up by 1%, re-price and give back the change in NPV. Because most exotic derivatives do involve more than one underlying, 
the NVega will move all volatility surfaces of all the underlying, with the exception of the FX underlying volatilities.


The key model assumptions for Bond Option are

•	There are no taxes, margins or transaction costs. This assumption is commonly accepted in the industry.
•	The underlying bond forward price follows a lognormal distribution. This assumption is commonly accepted in the industry.
•	The risk-free interest rate is constant This assumption is reasonable in the real world and commonly accepted in the industry.
•	The valuation methodologies assume there is no arbitrage. The no-arbitrage assumption makes it possible to state the price of an asset in terms of risk-neutral probabilities where the discounting is done at 
the risk-free rate. This is commonly used and universally accepted in both the industry and the academic world.



References:

[Cross rate](https://www.researchgate.net/publication/385275783_Modeling_Term_Structure_of_Cross-_Currency_Interest_Rates)

[Interest rate](https://www.researchgate.net/profile/Tim-Xiao/publication/385275783_Modeling_Term_Structure_of_Cross-_Currency_Interest_Rates/links/671d479dacba566ad501e638/Modeling-Term-Structure-of-Cross-Currency-Interest-Rates.pdf)







