
### Curve Construction Guide

The term structure of interest rates, also known as yield curve, is defined as the relationship between the yield-to-maturity on a zero coupon bond 
and the bond's maturity. Zero yield curves play an essential role in the valuation of all financial products. 

The current methodology in capital markets for marking to market securities and derivatives is to estimate and discount future cash flows using rates 
derived from the appropriate term structure. The yield term structure is increasingly used as the foundation for deriving relative term structures and 
as a benchmark for pricing and hedging. 

We adopt a hybrid of bootstrapping method and enhanced method to generate zero curve.  Assuming cash Libor rates, Libor futures and Libor swaps as 
underlying instruments, the curve generation process is described

Separate the underlying instruments into two groups based upon the longest Libor maturity of the corresponding Libor future.  Those with shorter maturities 
are classified as short to medium-term instruments; typical of cash Libor rates, Libor futures and short-term Libor swaps.  Those with longer maturities are 
long-term instruments; typical of medium to long term Libor swaps.

Yield curves can be derived from government bonds or LIBOR/swap instruments. The LIBOR/swap term structure offers several advantages over government 
curves, and is a robust tool for pricing and hedging financial products. Correlations among governments and other fixed-income products have declined, 
making the swap term structure a more efficient hedging and pricing vehicle. 



Reference:

[Curve Construction](/CurveConstruction-3.pdf)

[FlipHtml5 curve construction](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamgTO0MTM3ITPkl0av9mY)

[Zenodo curve construction](https://zenodo.org/record/6498116#.YpOvBqgpBD8)

[OSF curve construction](https://osf.io/evzp4/download)

[OSF variable swap](https://osf.io/j3p7q/wiki/home/)

[OSF variable rate swap](https://osf.io/np5bw/download)
