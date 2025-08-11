
###	Workflow Context 

Workflow Templates are designed and are defined by a set of Workflow States, Workflow Transitions, and associated Workflow Actions. Users interact with a particular Workflow Instance, and each Instance is created 
from a Workflow Template.

Workflow Template can be designed, such that workflow states, transitions, actions, and rules can be created/updated/deleted. Workflow Instance Users are able to participate within a Workflow Instance and can cause 
transitions and actions to occur.

The term delete shall mean: indicate as no longer active, not physically deleted.  Any deleted entity shall still be retrievable up to the retention period.

A configurable set of filter rules shall mean: Filter rules shall be based on meta-data driven constructs, using SDR catalogues to define the business logic and simple comparison operators. 
1.	Examples of simple comparison operators include “>=”, “=”, “AND”, “OR”, and “IN”. 
2.	Groups. It will be possible to define groups of a set of parameters for the purposes of applying filter rules, e.g. set up a list of the usernames for all users who are in the Credit Models team.
3.	The specific functionality is defined in the DRS documents for Data requirements, however applications are described here.

Workflow Instance Attributes are a set that includes:
1.	The values in the database record for a given workflow instance, i.e. values in the respective entry in the tables WF_Step_F, and WF_Instance_F.
2.	The values in the RDR record of the Object being approved.



References:

[osf pdf](https://osf.io/k3wc9/download)

[zenodo carc vol](https://zenodo.org/record/7487163)

[zenodo carc vol pdf](https://zenodo.org/record/7487163/files/CarcVolSurface.pdf)

[zenodo two carc](https://zenodo.org/record/7480149)

[zenodo two carc pdf](https://zenodo.org/record/7480149/files/TwoWayCarc.pdf)



