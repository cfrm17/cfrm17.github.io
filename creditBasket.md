
### Credit Basket Analysis 


TThe model is used to analyze the dynamics of a well diversified credit basket of names. More specifically, the tool is capable of predicting correlated loss levels and pool spreads over time. These forecasts can be used to further gauge the possibility of hitting predefined spread trigger thresholds.

A key motivation is the fact that certain trades have critical transaction triggers which reference these values. For example, Leveraged Super Senior (LSS) deals may trigger actions once the pool spread of an underlying CDX basket of 125 investment grade names reaches a specified threshold for a given loss level and remaining term.

In the model, names are allowed to migrate ratings on an individual basis according to a credit transition matrix. At the same time, spreads are simulated using mean reverting processes with time dependent parameters. For the purpose of spread evolution, names are grouped into classes of similar credit ratings. This classification simplifies the number of inputs required. Time dependent process parameters allows the inclusion of a spread term structure if desired.

Overall, this model captures the combined stochastic behaviour of both name migrations and spread forecasts. To ensure consistency, all dynamic processes are appropriately correlated with one another. Ultimately, at any simulated time the current basket loss level and pool spread can be used to check for trigger breaches. The portion of first trigger breaches relative to the number of simulated paths is an important measure. It represents an estimate of the probability of ever experiencing a spread trigger breach.

Calibration of this model may be a challenge given the number of correlated inputs and limited historical credit data. In this report we essentially test submitted inputs. In particular, we rely on the provided credit transition matrix and spread mean reverting parameters. On the other hand, we do investigate shocked scenarios as one way of assessing the sensitivity of the output to the supplied inputs.


Predicting an aggregate basket spread is highly non-trivial owing to the dynamics of the situation. The contribution to the overall spread from an individual name with a fixed credit rating is a stochastic process. On top of this, the credit rating of a given name may change at any time, despite there being no changes to the spreads of other names with similar ratings. Furthermore, all movements are correlated. That is, spreads are correlated with one another, migrations are correlated with one another and spreads are correlated with migrations. 

In order to forecast the basket loss level and pool spread it is essential to consider the combined effect of both spread and credit rating movements together. The proposed approach captures systemic risk, through grouped credit spread evolution, as well as idiosyncratic risk, through specific name migrations.


References:

[Articles](https://authors.repec.org/pro/pwh61/)

[More](http://citec.repec.org/p/w/pwh61.html)

[Research Gate](https://www.researchgate.net/profile/Tim-Xiao/publication/369898784_Convertible_Bond_Model_with_Soft_Call/links/6431a429ad9b6d17dc44cea0/Convertible-Bond-Model-with-Soft-Call.pdf)