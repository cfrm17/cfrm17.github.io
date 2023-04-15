## FX Derivatives


### FX Variance Swap

Variance swap does not have any dependence on spot FX rate and provides pure exposure to volatility alone. Thus, delta is zero for variance swap unless there is currency risk involved where the payoff settles in underlying currency. Vega and Rho calculations are also tested.


References: 


[Zenodo FX Variance Swap pdf](https://zenodo.org/record/7301706/files/FxVarianceSwap.pdf)

[Zenodo FX Variance Swap](https://zenodo.org/record/7301706)

[Git FX Variance Swap](https://github.com/cfrm17/fxVarianceSwap)


### CARC Option

We propose a Monte Carlo (Gaussian MC and Quasi MC) pricing model for the product named capped-accumulated-return-call (CARC) with lock in feature.  The new feature is represented by an increasing series of attributes 

References: 

[Zenodo CARC Option pdf](https://zenodo.org/record/7301746/files/CARCLockIn.pdf)

[Zenodo CARC Option](https://zenodo.org/record/7301746)

[Github CARC Option](https://github.com/cfrm17/carcLockIn)


### Double Window Double Barrier Option 

We offer a hybrid (trinomial tree plus semi-analytic formulas) pricing method for the product. Currently, the model uses spot implied volatility for the first time window, and forward implied volatility for the second time window. These are Black-Scholes implied volatilities from traded vanilla European options, but, while desired, usage of different volatilities based on strike or barrier moneyness directly within the tree is difficult to achieve. 

We will start by defining Single Knock Out Partial Barrier Option, Single Knock In Barrier Option, Double Knock Out Partial Barrier Option, and Double Knock In Barrier Option contracts on whose features the Double Window Double Barrier Option contract definition is based. The exercise style is assumed European everywhere in this paper.

References: 

[Zenodo Double Barrier Option pdf](https://zenodo.org/record/7301763/files/DoubleWindowDoubleBarrierOption.pdf)

[Zenodo Double Barrier Option](https://zenodo.org/record/7301763)

[Github Double Barrier Option](https://github.com/cfrm17/doubleWindowBarrier)


### Commodity Futures Swap 

Let us consider crude oil as an example of commodity. In the crude oil exchange market, futures contracts are available for each calendar month. The roll over dates for MAY-99 and JUN-99 futures contracts are 20-Apr-99 and 20-May-99, respectively. If t1 = 15-Apr-99, t2 = 20-Apr-99 and t3 = 21-May-99, Then the nearest futures for t1 and t2 is the MAY-99 contract, i.e., I(t1) = I(t2) = MAY-99, and the nearest futures for t3 is the JUN-99 contract, i.e., I(t3) = JUN-99.

References: 

[Zenodo Commodity Futures Swap pdf](https://zenodo.org/record/7308888/files/CommodityFutureSwap.pdf)

[Zenodo Commodity Futures Swap](https://zenodo.org/record/7308888)

[Github Commodity Futures Swap](https://github.com/cfrm17/cmcFutureSwap)


### Commodity Futures Swaption 

It is also assumed that the commodity price and the currency exchange rate follow geometric Brownian motions with deterministic volatilities. The correlative coefficient between the commodity futures and the exchange rate is assumed to be constant. Applying Vorst’s approximation

References: 

[Zenodo Commodity Futures Swaption pdf](https://zenodo.org/record/7308915/files/CommodityFutureSwaption.pdf)

[Zenodo Commodity Futures Swaption](https://zenodo.org/record/7308915)

[Github Commodity Futures Swaption](https://github.com/cfrm17/cmcFutureSwaption)


### FX Fade Option 

A fade option is a vanilla option that exists or dies if a barrier is breached on a single preset date, which is prior or equal to the contract maturity. Therefore, the barrier type can be up-cross or down-cross; the exercise type can be knock-in or knock-out; and the underlying vanilla can be call or put.

References: 

[Zenodo Commodity Futures Swaption pdf](https://zenodo.org/record/7313954/files/FaderIn.pdf)

[Zenodo Commodity Futures Swaption](https://zenodo.org/record/7313954)

[Github Commodity Futures Swaption](https://github.com/cfrm17/FadeOption)


### FX Option Delta 

If we want a scenario price where we assume a different spot FX, then the ingredients for pricing the new scenario option will be: new spot FX, time to expiry (as original), strike (as original), domestic foreign interest rate (as original), foreign interest rate (as original), and volatility extracted from smile using all these five parameters (this volatility will clearly be different from the volatility extracted in the original case as in the extraction process we are using a different spot FX rate).
 
 References: 
 
[Zenodo FX Option Delta pdf](https://zenodo.org/record/7314052/files/FxOptionDelta.pdf)
 
[Zenodo FX Option Delta](https://zenodo.org/record/7314052)
 
[Github FX Option Delta](https://github.com/cfrm17/FxOptionDelta) 


### Asian Futures Option 

The Asian option on futures is of European type vanilla arithmetic average call/put option on futures
prices. The term of “vanilla arithmetic average” means that weighting factors in the average are of
constant and positive. The matured payoff of the Asian option is the arithmetic average of one or several
futures prices over a preset period of reset time points. Assume the current time is zero. 

References: 

[Zenodo FX Asian Futures Option pdf](https://zenodo.org/record/7314403/files/FxAsianFutureOption.pdf)

[Zenodo FX Asian Futures Option](https://zenodo.org/record/7314403)

[Github FX Asian Futures Option](https://github.com/cfrm17/FxAsianFuturesOption)


### Power Swap

PWR-PHYS contracts are valuated as a swap of basket of indices, evaluating each buy/sell contract separately in the book (no matter of your buy/sell total portfolio strategy). Before maturity, the system treats the outstanding physical leg of the contract as another index (called POWER in the system). Before maturity this index is equal to the spot index at the point of delivery and after delivery the POWER index is set to 0. Thus the system assumes the entire portfolio of physical buy/sell contracts is balanced in terms of physical delivery at settlement time.

References: 

[Zenodo Power Swap pdf](https://zenodo.org/record/7314483/files/PowerSwap.pdf)

[Zenodo Power Swap](https://zenodo.org/record/7314483)

[Github Power Swap](https://github.com/cfrm17/PowerSwap)


### Ratio Tunnel Option 

A ratio tunnel option is defined as a European vanilla option upon a European collar. It is another special case of a general compound option. We can get a close form pricing formula for the option on collar, or the ratio tunnel option. Most of results presented in the report (see footnote 1) can be applied here. Therefore, in the following, we just provided some specified information which is necessary in this case.

References: 

[Zenodo Ratio Tunnel Option pdf](https://zenodo.org/record/7317139/files/RatioTunnelOption.pdf)

[Zenodo Ratio Tunnel Option](https://zenodo.org/record/7317139)

[Github Ratio Tunnel Option](https://github.com/cfrm17/RatioTunnelOption-)


### Reciprocal Average Rate Forward

The pricing model for the reciprocal average rate forward, in the view of a first order approximation, applies the same approach as in ordinary average rate forward. Pricing average rate related non-linear derivatives, a well-acceptable and effective with reasonable accuracy pricing model for the reciprocal average rate forward is not available yet.

We did some research of seeking a semi-close form solution for pricing non-linear average rate derivatives. This research has revealed satisfactory results for pricing linear reciprocal average rate derivatives 

References: 

[Zenodo Ratio Tunnel Option pdf](https://zenodo.org/record/7317169/files/ReciprocalAverageForward.pdf)

[Zenodo Ratio Tunnel Option](https://zenodo.org/record/7317169)

[github Ratio Tunnel Option](https://github.com/cfrm17/ReciprocalAverageRateForward)


### Compound Option 

A vanilla compound option is defined as a European vanilla option upon another European vanilla option,
which may be called underlying vanilla option. There are four types of compound options: call-on-call,
call-on-put, put-on-call and put-on-put. Due to the call-put parity, basically, we only need to consider call-on-call and call-on-put. In this report, under the assumption that the asset price, which is the underlyer of the underlying option, follows geometrical Brownian motion and that risk-free short rate, dividend yield and volatility are deterministic, we present Black-Scholes/Merton’s analytical close form pricing formula for vanilla compound options.

References: 

[Zenodo Compound Option pdf](https://zenodo.org/record/7317234/files/compoundOption.pdf)

[Zenodo Compound Option](https://zenodo.org/record/7317234)

[Github Compound Option](https://github.com/cfrm17/CompoundOption)


### Broker Strangle Algorithm 

The algorithm consists of solving a system of non-linear equations. When Left Delta quotation is used, nested non-linear equations are obtained as Left Delta leads by itself to solving a non-linear equation 

Let us fix an anchor term and corresponding foreign and domestic interest rates (they will not appear in our notation, but they are crucial in this algorithm along with volatility data).

References: 

[Zenodo Broker Strange Algorithm pdf](https://zenodo.org/record/7317278/files/BrokerStrangleAlgorithm.pdf)

[Zenodo Broker Strange Algorithm](https://zenodo.org/record/7317278)

[Zenodo Broker Strange Algorithm](https://github.com/cfrm17/BrokerStrangleAlgorithm)


### Single Fixing Barrier Fade Option 

Fade Option is priced under standard Black-Scholes assumptions with at-the-money (ATM) volatility term structure. Volatility skew is not accounted for and, consequently, these theoretical prices may be different from market ones. Moreover, In/Out parity can induce internal arbitrage (Fade In plus Fade Out add up to a Vanilla that is not on volatility smile as it should).

When the fixing date coincides to expiry date the Fade option payoff (also called European Barrier Option payoff) can be exactly replicated with European Vanilla and European Digital Options. As both Vanilla and European Digital Options can be consistently priced with volatility smile, a Fade Option with fixing at expiry can consequently be priced with smile. 

References: 

[Zenodo Gingle Fixing Barrir pdf](https://zenodo.org/record/7320191/files/SingleFixingBarrier.pdf)

[Zenodo Gingle Fixing Barrir](https://zenodo.org/record/7320191)

[Github Gingle Fixing Barrir](https://github.com/cfrm17/SingleFixingBarrier)


### Touch Option 

Let t S be the spot FX rate of a currency pair FOREIGN/DOMESTIC (FOR/DOM, f/d) at time t. In the FOR/DOM notation scheme, when one considers, for example, the EUR/USD-spot Skew Touch Model, say, at 1.26 USD per 1 EUR, the currency USD is used to measure 1 EUR, therefore we say that EUR is the underlying (the asset, the foreign currency) and USD is the numeraire (the domestic currency) used to value the asset 1 EUR. Another example: consider USD/JPY-spot trading, say, at 116 JPY per 1 USD; the currency JPY is used to measure 1 USD, so USD is the underlying (the asset, the foreign currency), and JPY is the numeraire (the domestic currency).

Let T be the time (in years) from current date (valuation date) to expiry date, shortly called time to expiry. Let be the time (in years) from spot date to delivery date, shortly called time to delivery. Let be the domestic interest rate (continuously compounded, ACT/365), the foreign interest rate (same conventions). Note that these rates apply from spot date to delivery date. Let d T d r f r σ be the volatility parameter (we think of it as a specification only in this section). The following continuous geometric Brownian process usually models the spot FX rate (here is the standard Brownian motion):

References: 

[Zenodo Touch Option pdf](https://zenodo.org/record/7348980/files/TouchOption.pdf)

[Zenodo Touch Option](https://zenodo.org/record/7348980)

[Github Touch Option](https://github.com/cfrm17/touchOption)
