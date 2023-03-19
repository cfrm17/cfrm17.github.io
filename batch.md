
### End of Day Process

Financial institutions have to perform Start of Day (SOD) process before it can carry out transactions for a specific date. Similarly, the End of Day 
(EOD) job must be run to process the transaction created during the day. When the scheduled EOD job completes, the system is advanced to the next date 
automatically. 

The EOD process can be performed manually, as well as automatically, as scheduled jobs through a job scheduler. The EOD jobs involved closing down daily 
activities, processing transactions and backing up all data.

Click the BatchRisk tab at the top-left corner of the application. Then, expend Batch -> Auto -> End of Day. If you created an auto end of day (EOD) 
scheduler already, it will be displayed in the main window.

A user can modify the scheduled time and then click the Save button to  save the changes. If the user have never created an auto EOD scheduler, 
he can click the New button. A new auto EOD template is displayed in the main window. Fill the time on which the user wants the EOD batch job to 
start daily and then click the Save button. A new auto EOD scheduler is created.

Click the BatchRisk tab at the top-left corner of the application. Then, expend Batch -> Manual and select End of Day.

A selection window pops up. You can select AllBooks or a particular leaf book (e.g., Interest Rate). All the EOD dates already generated in the system 
are displayed in the main window. You can either click the New button with a new Valuation Date to run a new EOD job right away or the Load button with 
a selected date to load existing EOD results.

If you input a new Valuation Date (e.g., 2/5/2018) at the top-right corner of the selection window and click the New button. FinPricing start to run 
the EOD for the book "Interest Rate" on 2/5/2018. The results are shown in the Result tab of the main window.

Note that all tradeIds in the results are underlined that means you can further drill down the results. Click a tradeId (e.g., T000000120010000026). 
The drill-down results are displayed in the DrillDownResult tab of the main window.


Referencce:

[Batch Process](/BatchJob-2.pdf)

[Zenodo eod](https://zenodo.org/record/6512443/files/Zenodo-BatchJob.pdf)

[Fliphtml5 eod](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamcDO0MTM3ITPkl0av9mY)

[OSF eod](https://osf.io/4q3tf/download)

[OSF inverse swap](https://osf.io/9jyh8/download)

[Github balance](https://github.com/cfrm17/BalanceSheetRisk)

[Github cms cliqust](https://github.com/cfrm17/CMSCliquet)
