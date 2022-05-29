
### Credit Valuation Adjustment

Credit Valuation Adjustment (CVA) is a tool in counterparty credit risk management and its application.  Counterparty credit risk is the risk that a counterparty 
to a financial contract will default prior to expiry, failing to make future contracts and resulting in a credit exposure to the financial institution.  Traditional 
methods of managing counterparty credit risk include netting agreements and collateralization to reduce the overall exposure to a single counterparty.  Over the past decade, 
institutions have also used Credit Default Swap (CDS) protection to manage exposures 

CVA, by definition, is the difference between the risk-free portfolio value and the true (or risky or defaultable) portfolio value that takes into 
account the possibility of a counterparty’s default. The risk-free portfolio value is what brokers quote or what trading systems or models normally 
report. The risky portfolio value, however, is a relatively less explored and less transparent area, which is the main challenge and core theme for CVA. 
In other words, central to CVA is risky valuation.

In the market, risk-free values are quoted for most financial derivatives. In other words, credit risk is not captured. Historical experience shows 
that credit risk often leads to significant losses. Therefore, it is obvious to all market participants that credit risk should be taken into account 
when reporting the fair value of any defaultable derivative. The adjustment to the risk-free value is known as the credit value adjustment (CVA).

More informally, think of CVA as the fair value of buying protection against the counterparty’s potential failure to meet contractual obligations.  From this 
perspective, calculation of CVA is a pricing exercise similar to option pricing.  In particular, because we are interested in the fair value of protection we 
can express the problem as the cost of hedging against default, allowing us to work in a risk-neutral measure in which the expected return of the hedged 
portfolio is the risk-free rate.  

For completeness, our theoretical study covers various cases. We find that the valuation of defaultable derivatives and their CVAs, in most situations, 
has a backward recursive nature and requires a backward induction valuation. An intuitive explanation is that two counterparties implicitly sell each 
other an option to default when entering into a defaultable transaction. If we assume that a default may occur at any time, the default options are 
American style options. If we assume that a default may only happen on the payment dates, the default options are either European options or Bermudan 
options. Both Bermudan and American options require backward induction valuations. 

Based on our theory, we propose a novel cash-flow-based practical framework for calculating the bilateral risky value and bilateral CVA at the counterparty 
portfolio level. This framework can easily incorporate various credit mitigation techniques, such as netting agreements and margin agreements, and can 
capture wrong/right way risk. Numerical results show that these credit mitigation techniques and wrong/right way risk have significant impacts on CVA. 


Reference: 

[CVA](/cva-4.pdf)

[FlipHtml5 cva](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamAjMwkzM5ITPkl0av9mY)

[FlipHtml5 cva pdf](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamYzM2IjNyETPkl0av9mY)

[Zenodo cva](https://zenodo.org/record/6533799#.YpOqwagpBD8)

[Hcommon cva](https://hcommons.org/deposits/download/hc:32984/CONTENT/cva-4.pdf)

[ScienceMedia cva](http://science-media.org/userfiles/1020/presentations/1020_presentation_436.pdf)

[Archive cva](https://ia801000.us.archive.org/32/items/alex_Cva_201804/cva-4.pdf)

[OSF cva](https://osf.io/hygf7/download)

