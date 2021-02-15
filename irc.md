
### Incremental Risk Charge

The incremental risk charge (IRC) is a regulatory requirement from the Basel Committee in response to the financial crisis. It supplements existing Value-at-Risk 
(VaR) and captures the loss due to default and migration events at a 99.9% confidence level over a one-year capital horizon. 

The liquidity of a position is explicitly modeled in IRC through liquidity horizon and constant level of risk. The constant level of risk is a new concept 
in IRC. It assumes banks hold portfolio constant over a liquidity horizon. At the beginning of the next horizon, they rebalance any default, downgraded, 
or upgraded positions and roll over any matured trades. This presentation describes methodology and implementation details of IRC. 

The Basel Committee on Banking Supervision (see Basel [2009 a]) released the new guidelines for Incremental Risk Charge (IRC) that are part of the new 
rules developed in response to the financial crisis and is a key part of a series of regulatory enhancements being rolled out by regulators.

IRC supplements existing Value-at-Risk (VaR) and captures the loss due to default and migration events at a 99.9% confidence level over a one-year 
capital horizon. The liquidity of position is explicitly modeled in IRC through liquidity horizon and constant level of risk.

The constant level of risk assumption in IRC reflects the view that securities and derivatives held in the trading book are generally more liquid than 
those in the banking book and may be rebalanced more frequently than once a year.  IRC should assume a constant level of risk over 
a one-year capital horizon which may contain shorter liquidity horizons. This constant level of risk assumption implies that a bank would rebalance, 
or rollover, its positions over the one-year capital horizon in a manner that maintains the initial risk level, as indicated by the profile of exposure 
by credit rating and concentration.

To caluclate IRC, one needs to simulate default and migration for one-year horizon. Also, one needs to take concentration into account, that measures 
the degree of a portfolio diversification. For example, if a significant number of issuers belong to a certain category, the portfolio is a concentrated 
one.


Reference: 

[IRC](/irc-9.pdf)

[Pubpub irc home](https://interestrate.pubpub.org/pub/469v839f/release/1)

[Pubpub irc pdf](https://assets.pubpub.org/z66vbt2h/31599313871841.pdf)

[Authorstream irc](http://www.authorstream.com/Presentation/tommills-4397631-incremental-risk-charge-irc-introduction/)

[Hcommon irc](https://hcommons.org/deposits/download/hc:33530/CONTENT/irc-9.pdf)

[FlipHtml5 irc](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamEDM2UDN5ITPkl0av9mY)

[Github irc](https://github.com/cfrm17/irc/raw/main/irc-9.pdf)

[Pubpub irc](https://interestrate.pubpub.org/pub/469v839f/download/pdf)

[Zenodo irc](https://zenodo.org/record/4025375/files/irc-9.pdf)

[Bitbucket irc](https://bitbucket.org/cfrm17/irc/downloads/irc-9.pdf)

[Gitlab irc](https://gitlab.com/cfrm171/irc/-/raw/master/irc-9.pdf)

[Archive irc](https://ia601401.us.archive.org/13/items/irc-9/irc-9.pdf)

[OSF irc](https://osf.io/4fdjm/download)
