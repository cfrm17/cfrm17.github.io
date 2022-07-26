## Financial Market Analysis


### Derivatives Pricing Models

[Reference](https://finpricing.com/FinPricing-ProductBrochure.pdf)



### Ratchet Swap

A ratchet swap is an interest rate swap with two legs. One leg is a standard floating leg and the other leg is a ratchet leg. The ratchet leg pays a ratchet floating rate.

The ratchet floating rate coupon is based on an index, e.g., 6-month EURIBOR. The rate is further subject to a minimum decrease of 0 bps and a maximum increase of a threshold, such as, 15 bps. These rates are reset two business days prior to the first day of each coupon period. 



References: 

[OSF ratchet swap](https://osf.io/azy78/download)



### Hull-White Volatility Calibration

In Black’s framework, a European swaption is at the money if the strike level is equal to the forward swap rate. In this case, the prices of a payer and a receiver swaption on the same underlying swap will be equal. 

Mortgages are mapped to short rate volatilities, in order to value the embedded prepayment option. An open mortgage is a mortgage that allows the mortgagee to refinance at any time after a specified date; we will call this date the first exercise date.

Hull-White (HW) short interest rate volatilities are calibrated via at the money European swaptions. 


References: 

[OSF HW vol](https://osf.io/q6sv3/download)



### Quanto CMS Spread Swap

A quanto CMS spread swap is an exotic interest rate swap. The swap consists of two legs: One leg is a fixed rate leg. The other leg pays a fixed rate during a portion of the tenor and a variable rate during the remaining part. The variable rate is based on a spread between GBP and EURO 10 year CMS rates. Depending on the deal, the floating rate payments may last up to 20 years.


References: 

[OSF HW vol](https://osf.io/umeq3/download)


### LIBOR Rate Model

LIBOR Rate Model is used for pricing Libor-rate based derivative securities. The model is applied, primarily, to value instruments that settle at a Libor-rate reset point.  In order to value instruments that settle at points intermediate to Libor resets, we calculate the numeraire value at the settlement time by interpolating the numeraire at bracketing Libor reset points. 


References: 

[OSF HW vol](https://osf.io/wra62/download)

