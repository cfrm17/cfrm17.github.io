
### Hull White Volatility Calibration

Hull White model is a short rate model that is used to price interest rate derivatives, such as Bermudan swaption and accumulator exotics (see https://finpricing.com/lib/FxAccumulator.html)

We map implied Black's at the money (ATM) European swaption volatilities into corresponding Hull-White (HW) short rate volatilities. We seek to determine a HW volatility to match the market 
price of a certain ATM European payer swaption.  


We present an approach that calculates the HW volatility to make the swaption price calculated on a HW tree match Black's price for the same swaption at each grid point.

At each grid point, we compared respective Black’s and HW trinomial tree payer swaption pricing benchmarks. Specifically, using the interest rate and implied Black’s volatility .

We priced the payer swaption using our benchmark Black’s model and then priced the same swaption, using our benchmark HW trinomial tree model, based on the corresponding HW volatility.

We found close agreement in the two benchmark prices above; however, for short swaption tenors and swap terms, the agreement between these two prices was only marginally acceptable.



References:

[osf pdf](https://osf.io/k3wc9/download)

[zenodo multi carc](https://zenodo.org/record/7480124)

[zenodo multi carc](https://zenodo.org/record/7480124/files/MultiCarc.pdf)

[zenodo two carc](https://zenodo.org/record/7480149)

[zenodo two carc](https://zenodo.org/record/7480149/files/TwoWayCarc.pdf)



