.. Introduction:

1. Introduction
=====================================

1.1 Projects overview
+++++++++++++++++++++++
The creation of the Sierra Leone OSeMOSYS and MAED models started as part of an effort from Climate Compatible Growth, at the invitation of the Presidential Initiative on Climate Change, Renewable Energy and Food Security (PI-CREF), to capacitate the Planning Unit in the Sierra Leone Ministry of Energy (MoE).

The project consisted of a team of researchers from CCG and the MoE's Planning Unit. Through the co-creation of an Energy System Optimisation Model (ESOM), skills were shared and transferred between the members of the team allowing for the continuation of energy modelling in Sierra Leone.


1.2 Motivation and problem statement
+++++++++

1.3 The Model for the Analysis of Energy Demand (MAED)
++++++++++++++++++++++++++++++++++++++++++++++++++++++++

1.4 The Open Source energy Modelling System (OSeMOSYS)
++++++++++++++++++++++++++++++++++++++++++++++++++++++++

OSeMOSYS is an optimization software for long-term energy planning. It is an open source model structured in blocks of functionality that allows easy modifications to the code, providing a great flexibility for the creative process of the solution. The models that are built in OSeMOSYS minimize the total cost of the system for a certain period of time, defining the configuration of the supply system, considering some restrictions on activity, capacity, and emissions of technologies :cite:`HOWELLS20115850`. This is shown in the following equation: 

.. math::

   Minimize \sum_{y,t,r}Total\ discounted\ cost_{y,t,r},
   
where: *y* corresponds to the year, *t* to the technology and *r* to the region. 

The discounted cost can be expressed as follows: 

.. math::

   \forall _{y,t,r}\  Total\ discounted\ cost_{y,t,r}\  =   DOC_{y,t,r} + DCI_{y,t,r}  + DTEP_{y,t,r} - DSV_{y,t,r},
 
where: 

*	*DOC (Discounted Operational Cost):* Corresponds to the cost related to maintenance (fixed, usually associate to capacity) and operation of technologies (variable, linked to fuel uses and level of activity).  
*	*DCI (Discounted Capital Investment):* It is the cost of investment of all technologies selected to supply energy on the whole period. 
*	*DTEP (Discounted Technology Emission Penalty):* It is associated to the use of pollutants. The calculation is based on the emission factor and the activity of technologies and the specific cost by pollutant.    
*	*DSV (Discounted Salvage Value):* As the capital cost is discounted in the first year a technology is acquired, if in the last year of study the technologies have remaining years of operational life, the corresponding value is counted.

1.5 Robust Decision Making (RDM)
++++++++++++++++++++++++++++++++++++++++++++++++++++++++