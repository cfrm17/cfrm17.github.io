## Derivatives Valuation

### GIC Pooling

The payoff at maturity from a GIC can be shown equal to the invested principal plus these principal times the sum of the minimum guaranteed interest rate and the payoff from a European 
call option on the arithmetic average of a basket price at the 12 points above, where the basket price is given by a weighted sum of the index levels above.  


[Reference:](/gicPooling.md)

[ois pdf](https://osf.io/atyb9/download)



### Quanto Himalayan Option 

Himalayan options are a form of European-style, path-dependent, exotic option on a basket of equity underliers, in which intermediate returns on selected equities enter the payoff, while the
equities are subsequently removed from the basket.


[Reference:](/quantoHimalayan.md)


### Local Volatility Model for Callables 

We review a model for computing the price, in the domestic currency, of European standard call and put options on an underlying foreign equity (stock or index) with tenor of up to 7 years. 
The function implements a local volatility based pricing method.


[Reference:](/localVolQuanto.md)


### Forward Starting Option Valuation 

Forward start option is an option whose strike will be determined at some later date. Unlike a standard option, the strike price is not fully determined until an intermediate date before 
expiration. Cliquet option consists of a series of forward start options. 


[Reference:](/forwardStart.md)

[ois pdf](https://osf.io/37fbt/download)


### Three Factor Convertible Bond Model

The owner of a convertible bond (CB) receives periodic coupon payments from the issuer, but can also convert the CB into the issuer’s stock.  The convertible bond may also include call 
and put provisions, which respectively allow the issuer to buy back the convertible bond and the owner to put the convertible bond for respective preset amounts.  


[Reference:](/threeFactorConvertible.md)


### Mutual Fund Securitization Model

The purpose of the model is to determine, from a projected stream of future cashflows, whether all Commercial Paper used to fund the commissions to brokers for the sale of mutual funds 
will be repaid within a period.  Here a broker charges the Partnership a commission on the net asset value of the mutual funds sold.  The buyer of the mutual funds, however, pays nothing 
up front; instead, a deferred sales charge, which depends on when the mutual funds are redeemed, is assessed.


[Reference:](/mfSecuritization.md)


### Pricing Convertible Bond via Hull White Model

Using the Hull-White two-factor tree building procedure, a combined tree is constructed by matching the mean, variance and correlation corresponding to each combined tree node.  
The convertible bond price is given from the combined tree by backward induction.  


[Reference:](/hwConvertible.md)


### Brownian Bridge Approach

The Brownian bridge algorithm has been implemented for stress testing within the Risk Management framework. It is used for generation of multidimensional random paths whose initial and ending 
points are predetermined and fixed. 


[Reference:](/brownianBridge.md)

[osf pdf](https://osf.io/6dn54/download)



### Exchangeable Convertible Bond Model

A convertible bond issuer pays periodic coupons to the convertible bond holder. The bond holder can convert the bond into the underlying stock within the period(s) of time specified 
by the conversion schedule. The bond issuer can call the bond and the holder can put it according to the call and put provisions. 


[Reference:](/exchangeableConvertible.md)

[osf pdf](https://osf.io/zgx8c/download)




### Asset Backed Senior Note Valuation

We consider a securitization deal, which allows the holder to purchase co-ownership interests in a revolving pool of credit card receivables. To fund the acquisition of the interests in the revolving pool, 
the trust issued Asset-Backed Notes, in a number of different series. A share of future collections of credit charge receivables, to which the trust is entitled, is used to pay the interest and the 
principal of the notes.


[Reference:](/absSenior.md)

[pdf](https://osf.io/eg6mv/download)


### Hull White Volatility Calibration

Hull White model is a short rate model that is used to price interest rate derivatives, such as Bermudan swaption and accumulator exotics 


[Reference:](/hwVol.md)



### Bond Bootstrapping Approach

We discuss a method for bootstrapping a set of zero rates from an input set of US government money market securities and bonds. The government bond bootstrapping procedure requires to input a set of 
financial instruments, of the type below, sorted by order of increasing time to maturity:


[Reference:](/bondCurve.md)

[pdf](https://osf.io/4nhyb/download)



### GIC Valuation

Guaranteed investment certificate (GIC) is a financial instrument that offers a return based on a corresponding GIC rate and the performance of a basket of certain stock and bond market indices. 


[Reference:](/gicPricing.md)

[ois pdf](https://osf.io/tgd82/download)



### Extendable Swap Valuation

We use analytical formulas for forward swap and swaption valuation: the swap price is calculated as the difference between a bond par and the bond’s price, and the swaption price is evaluated from the Black’s formula.


[Reference:](/extendableSwap.md)

[osf pdf](https://osf.io/23w9h/download)



### Callable Inverse Swap Valuation

A Callable Inverse Floating Rate Swap is a forward swap agreement with an option of canceling the swap each year starting from several years in future. The deal is priced with a two factor Black-Karasinski model.

[Reference:](/callableInverse.md)

[osf pdf](https://osf.io/9jyh8/download)



### Flexible GIC Valuation

A flexible GIC is an investment with an embedded option to redeem the principal and accrued interest at any time after 30 days from the date of purchase. In other words, the holder of GIC has an option to redeem 
the principal and accrued interest at any time after 30 days of from the date of purchase. No interest is paid if the investment is redeemed within first 30 days from the purchase date.

[Reference:](/flexibleGic.md)

[osf pdf](https://osf.io/q6ut7/download)



### American Bond Option Pricing

Pricing an American style call option on the yield of Treasury bond is discussed. The payoff is positive if the yield exceeds a predetermined strike level. The model assumes the yield of an American Treasury bond to be a log-normally distributed stochastic process and uses Monte-Carlo simulation to price the deal as a European call option. 

[Reference:](/americanBond.md)

[pdf](https://osf.io/q6ut7/download)


### Martingale Preserving Tree 

An important feature of the popular three factor trinomial tree is that it uses a deterministic approximation of the interest rates for constructing the stock tree. The preservation of the martingale property of the stock price is thus not guaranteed.  and may potentially represent a problem.Pricing an American style call option on the yield of Treasury bond is discussed. The payoff is positive if the yield exceeds a predetermined strike level. The model assumes the yield of an American Treasury bond to be a log-normally distributed stochastic process and uses Monte-Carlo simulation to price the deal as a European call option. 

[Reference:](/preservingTree.md)


### Arrear Quanto CMS Valuation

Assumes that, under the coupon payment currency (SEK) risk-neutral probability measure, the forward swap rate process corresponding to each swap rate fixing follows Geometric Brownian motion with drift.  Each forward swap rate process is then convexity adjusted, and is furthermore expressed under the notional currency (FRF) risk neutral-probability measure by means of a quanto adjustment.

[Reference:](/arrearCms.md)

[pdf](https://osf.io/g6tp5/download)


### Variable Rate Swap Valuation

Variable rate swap is a special type of interest rate swap in which one leg of the swap corresponds to fixed rate payments while the other involves fixed rate payments for an initial period of time and a floating rate for the rest. The floating rate on that portion is defined as a minimum of two index rates.

[Reference:](/variableSwap.md)


### CMS Spread Option Valuation

A constant maturity swap (CMS) spread option makes payments based on a bounded spread between two index rates (e.g., a GBP CMS rate and a EURO CMS rate).  The GBP CMS rate is calculated from a 15 year swap with semi-annual, upfront payments, while the EURO CMS rate is based on a 15 year swap with annual, upfront payments. 

[Reference:](/cmsSpread.md)

[pdf](https://osf.io/9db5u/download)



### Early Start Swap Valuation

An early start swap is a swap that has an American style option for the counterparty of starting the swap early, within a period of three month. Otherwise, the swaps are plain vanilla fixed-for-floating swaps.

[Reference:](/earlySwap.md)

[ois pdf](https://osf.io/kapm3/download)



### Quanto TRS Valuation

A quanto total return Libor Swap is a swap where one leg is a regular floating leg paying LIBOR less a constant spread and the other leg makes a single payment at the swap’s maturity equal to a leveraged non-negative return on USD-for-EURO exchange rate paid in CAD. The main focus of the valuation model is the quantoed total return on the FX rate.

[Reference:](/quantoTrs.md)



### Digital Swap Valuation

A daily digital LIBOR swap is an interest rate swap whose reference interest rate is three-month USD Libor BBA. For each accrual period in the swap, one party receives the reference rate, and pays the reference rate plus a positive spread, but weighted by the ratio of the number of calendar days in the period that the reference rate sets below an upper level to the total number of calendar days in the period.

[Reference:](/digitalSwap.md)

[ois pdf](https://osf.io/qzmer/download)



### Ratchet Swap Valuation

The ratchet floating rate coupon is based on an index, e.g., 6-month EURIBOR. The rate is further subject to a minimum decrease of 0 bps and a maximum increase of a threshold, such as, 15 bps. These rates are reset two business days prior to the first day of each coupon period. 

[Reference:](/ratchetSwap.md)



### LIBOR Rate Model 

LIBOR Rate Model is used for pricing Libor-rate based derivative securities. The model is applied, primarily, to value instruments that settle at a Libor-rate reset point.  In order to value instruments that settle at points intermediate to Libor resets, we calculate the numeraire value at the settlement time by interpolating the numeraire at bracketing Libor reset points. 

[Reference:](/liborModel.md)

