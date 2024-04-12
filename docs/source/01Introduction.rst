.. Introduction:

1. Introduction
=====================================

1.1 Projects overview
+++++++++++++++++++++++
The creation of the Sierra Leone OSeMOSYS and MAED models started as part of an effort from Climate Compatible Growth, at the invitation of the Presidential Initiative on Climate Change, Renewable Energy and Food Security (PI-CREF), to capacitate the Planning Unit in the Sierra Leone Ministry of Energy (MoE).

The project consisted of a team of researchers from CCG and the MoE's Planning Unit. Through the co-creation of an Energy System Optimisation Model (ESOM), skills were shared and transferred between the members of the team allowing for the continuation of energy modelling in Sierra Leone.

The goal of the team was to create an ESOM that focussed on the power sector in Sierra Leone and the costs and benefits, from a techno-economic perspecive, of various hydropower expansion plans in the country. In order to do this, a demand forecasting model, using the Model for the Analysis of Energy Demand (MAED), and central capacity expansion model, using the Open-Source Energy Modelling System (OSeMOSYS), were used. In order to validate the findings of the OSeMOSYS model, the Robust Decision Making framework was employed.

1.2 Motivation and problem statement
+++++++++
Sierra Leone's power sector currently relies heavily on hydropower to meet demand during the wet season. The 50 MW Bumbuna hydropower facility provides the majority of this generating capacity. However, during the dry season, due to a small reservoir, the capacity of Bumbuna is reduced to roughly 7 MW. Consequently, fossil fuel powered generators are relied upon during the dry season. A key contributor is the 66 MW Karpowership Heavy Fuel Oil (HFO) power barge. Asside from the nagetive environmental and social impacts of burning HFO for power generation, Karpowership has resulted in roughly $40 million of unpaid arreers.

Resulting from the existing Bumbuna site's shortfalls in providing reliable electricity generation capacity throughout the year, there are various plans to expand its generation capacity and/or construct an additional reservoir further upstream at a site called Yiben.

Sierra Leone has no economically recoverable fossil fuel reserves.

Electricity demand is expected to increase follwoing economic developement and electrification of households.

In this context, and through consultsation with the MoE, PI-CREF, and other key stakeholders, we can see that the sustainable expansion of Sierra Leone's power sector is a key priority for the government in order to mee the growing demand due to electrification and reduce reliance on fossil fuel power plants and their associated costs.

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