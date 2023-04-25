
### Dividend Exposure 


Dividend risk arises from dividend uncertainty, mostly coming from company idiosyncrasy. Like other type of market risk, the dividend risk is primarily due to market perception rather than actual performance of the underlying company. The equity derivatives that take expected dividend amount or yield as a pricing input are exposed to dividend risk.

The proposal is to capture the dividend risk under normal market conditions. Stress test is considered a more appropriate approach to capture the risk of severe cutting or eliminating dividend of large blue chip stocks during financial crisis.

We model one-day innovation in dividend expectation of a stock as a mixed distribution with two components: jumps and no jump. Jumps refer to non-zero innovation, modeled using double exponential distribution to account for fat tails. No-jump corresponds to the scenario that the dividend projection stays unchanged, typical for large utilities. For equity index, due to diversification we assume that the innovation is always non-zero. Thus, the one-day innovation in dividend expectation of an equity index is modeled using double exponential distribution. Baskets of stocks are mapped to equity index. Correlation among dividend of equity indices, as well as correlation between dividend risk factors and other risk factors, is also captured. We assume no correlation among the dividend of single stocks.

To calibrate the dividend risk factor, implied dividend yield from equity index futures market is investigated. However, we observe that the implied dividend yield is contract specific and predominantly driven by index price, which is already a risk factor. The innovation in expected dividend cannot be accurately estimated from implied dividend yield due to the large noise from market technicalities. This is evidenced by the extraordinarily high volatility (over 40%) of the daily innovation in dividend expectation. 

As an alternative, Bloomberg projected dividend amount is a forward-looking estimate based on multiple factors including market price of traded options. It is widely used by traders in pricing equity derivatives. We consider it appropriate to calibrate dividend risk model using Bloomberg projected dividend.


References:

[bitbucket pdf](https://bitbucket.org/timxiao1203/dividendexposure/downloads/DividendExposure.pdf)

[github compound](https://github.com/cfrm17/CompoundOption)

[github strangle](https://github.com/cfrm17/BrokerStrangleAlgorithm)

[github barrier](https://github.com/cfrm17/SingleFixingBarrier)
