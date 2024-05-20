4. OSeMOSYS model: Framework 
=======================================

This documentation has been created in order to provide an overview of OSeMOSYS-SL. Therefore, it presents the model structure, and gives a synthesis of the key assumptions of the model, regarding the numerical inputs used for the sets, parameters, and scenario building. First, in this section, we give an insight to the general framework of the model.

4.1 General model structure 
+++++++++

The Sierra Leonean energy sector is entirely modelled in OSeMOSYS. This has been built to focus on key concerns within the development of Sierra Leons's power sector, with key planned and prospective power plant projects such as the Bumbuna II (Yiben) modelled individually within the OSeMOSYS model. This model does not currently include demand or technologies driven by the transport sector in part due to a lack of available data. The overall structure of the model can be summarised in the simplified diagram Figure 2.1. with primary energy sourced from renewables, imported fossil fuels, domestic biomass or imported electricity. These commodities are transformed through a range of technologies to meet demands from different sectors as established in the MAED model, including Industrial, Commercial, and Residential household demands.  


.. figure:: img/SL_Mod_Struc.png 
   :align:   center
   :width:   700 px

*Figure 4.1: Simplified diagram for technologies within the Sierra Leone model*

4.2 Sets 
+++++++++

The sets are responsible for defining the structure of the model (i.e. temporal space, geographic space, elements of the system, etc.). In OSeMOSYS, the group of sets include: years, fuels, technologies, emissions and modes of operation. As is going to be further explained, the sets are characterised through parameters. These subsections present the sets that compose the current version of OSeMOSYS-SL.  

4.2.1 Year
---------

This corresponds to the period of analysis. For OSeMOSYS-SL it is from 2015 to 2050. However, the data from 2015 to 2023 is set according to historical information. 

4.2.2 Fuels
---------
In the OSeMOSYS model fuels act as commodities, with their availability often split between the demand of several technologies. These are crucial in establishing limitations in the supply chain of Sierra Leone's power sector from the three main fuel sources of production, importation or renewable fuels available for use in energy generation within Sierra Leone.  

4.2.3 Technologies
---------

.. figure:: img/SL_Technology_Diag.png
   :align:   center
   :width:   700 px

*Figure 4.1.3: Simplified diagram of the technology groupings used within the Sierra Leone OSeMOSYS model*

Groups of technologies represented in Figure 4.1.3 have been simplified from the technologies that can be found in the Annex section. A description of each grouping can be found below:

The first group, labelled IMP-PROD is used within the model to represent the availability and processing of raw commodities for use in energy generation within Sierra Leone. This can be directly in use in power plants as is the case with all renewables, as well as imported Heavy Fuel Oil (HFO) and Light Fuel Oil (LFO). However, for Crude Oil imports, this includes the processing of this to generate HFO and LFO fuels. 

The second grouping labelled PP-TD represents Sierra Leone's power sector infrastructure, including renewable and non-renewable power generation from raw commodities, the transmission and distribution, and the import of energy both internationally and from Karpowership.

The last grouping labelled as SECT represents the division of energy within Sierra Leone's sectors. This includes the use of some primary commodities such as biomass in heating and cooking which constitutes a large portion of Sierra Leone's energy use, as well as the division of fuels and energy within Sierra Leone's sectors. This is driven by the demands predicted by MAED for Sierra Leone's Residential, Industrial and Commercial sectors. 

Table 4.1.3 summarises these groupings in OSeMOSYS-SL.

+----------------+----------------------+-----------------------------------------------------------------------------------+
| Group          |Description           | Example                                                                           |
+================+======================+===================================================================================+
| IMP-PROD       | Energy Commodities   | Imported and domestic commodities (Fossil fuels, biomass and renewable resources) |
|                |                      | as well as their distribution and processing                                      |
+----------------+----------------------+-----------------------------------------------------------------------------------+
| PP-TD          | Power Plants and     | Solar power plants, hydro power plants, biomass power plants, energy imports and  |
|                | Grid Infrastructure  | transmission and distribution as well as specific power plants within Sierra Leone|
+----------------+----------------------+-----------------------------------------------------------------------------------+
| SECT           | Sectoral Divisions   | The use of fuels and energy within sectors for Sierra Leone currently modelled as |
|                |                      | Residential, Industrial and Commercial uses of energy and raw resources for       |
|                |                      | processes such as cooking and heating.                                            |
+----------------+----------------------+-----------------------------------------------------------------------------------+

4.2.4 Emissions
---------
This OSeMOSYS model focuses on accounting for the CO₂ emissions associated with the energy generating technologies as a key concern for Sierra Leone's climate initiatives. The addition of the transport sector in the modelling would further the national emissions. 

4.2.5 Mode of operation
---------
The model has one mode of operation, for representing the normal operation of the system. Scenario design can be found in Section 6.   

4.2.6 Region
---------

The model has a nationwide scope, therefore it only has one region: Sierra Leone (SL).
