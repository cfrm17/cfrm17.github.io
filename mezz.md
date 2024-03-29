
### MezzMezzMezz Trade 


The MezzMezzMezz trade model is a synthetic Collateral Debt Obligation (CDO) structure in which the collateral pool is composed of tranches issued under MezzOfMezz or Caribou structures. Each participating MezzOfMezz tranche is a CDO mezz tranche defined by a threshold and a principal. Several such MezzOfMezz tranches are aggregated and tranched into MezzMezzMezz tranches. Within the existing modelling framework the model is implemented by adding a layer of CDO structure to the MezzOfMezz model.

The MezzMezzMezz or Mezzcubed trade model implements a trade structure in which the tranches defined by MezzOfMezz or Caribou structures are aggregated under a new Collateral Debt Obligation (CDO) structure. The synthetic CDO trade models used by the  system are FirstLoss, MezzOfMezz, and MezzMezzMezz. The following diagrams show how these models are structured

Within the existing modeling framework, the implementation of MezzMezzMezz trade is straightforward by adding a layer of CDO structure to the MezzOfMezz trade model. Instead of a direct aggregation and tranching of the mezz tranches of the participating CDO portfolios in MezzOfMezz trade model, in MezzMezzMezz trade model these initial mezz tranches are first aggregated into several MezzOfMezz structures. Each MezzOfMezz Structure (meta-CDO) is a CDO structure in which two or more mezz tranches of CDO portfolios are aggregated and tranched. All these meta-CDOs form a layer of CDO structure.   In this CDO layer the new mezz tranches, with each tranche defined by a threshold and a principal, are then aggregated and tranched into several MezzMezzMezz tranches.  

If there is no tranching in the meta-CDO structure and the principal is the full aggregation of all participating mezz tranches, MezzMezzMezz trade is reduced to a MezzOfMezz trade. We could replicate the results using MezzOfMezz trade model. Test trade one serves this purpose and the results generated by MezzMezzMezz trade model and MezzOfMezz model.

The submitted  MezzMezzMezz or Mezzcubed trade model implements a CDO trade structure in which the tranches issued under MezzOfMezz structures are aggregated under a new CDO structure. It is implemented by adding an intermediate layer of CDO structure to the MezzOfMezz trade model. Our tests have shown that the model is implemented in the way described in this report. The submitted results of the test trades agree with our independent implementation very well.


References:

[zenodo pdf](https://zenodo.org/record/7383005/files/MezzMezzMezz.pdf)

[archive correlation](https://ia803401.us.archive.org/11/items/eq-correlation-swap-26/EqCorrelationSwap-archive.pdf)

[gitbook cash](https://finwhite.gitbook.io/mortgagecashflow/)

[github black](https://github.com/timxiao1203/BlackOptionModel)

[github digital](https://github.com/timxiao1203/DigitalOption)
