4. OSeMOSYS model: framework 
=======================================

This documentation has been created in order to provide an overview of OSeMOSYS-SL. Therefore, it presents the model structure, and gives a synthesis of the key assumptions of the model, regarding the numerical inputs used for the sets, parameters, and scenario building. First, in this section, we give an insight to the general framework of the model.

2.1 General model structure 
+++++++++

TThe Sierra Leonean energy sector is entirely modelled in OSeMOSYS. This has been built to focus on key concerns within the development of Sierra Leons's power sector, with key planned and prospective power plant projects such as the Bumbuna II (Yiben) modelled individually within the OSeMOSYs model. This model does not currently include demand or technologies driven by the transport sector in part due to a lack of available data. The overall structure of the model can be summarised in the simplified diagram Figure 2.1. with primary energy sourced from renewables, imported fossil fuels, domestic biomass or imported electricity. These commodities are transformed through a range of technologies to meet demands from different sectors as established in the MAED model, including Industrial, Commercial, and Residential household demands.  

2.2 Sets 
+++++++++

The sets are responsible for defining the structure of the model (i.e. temporal space, geographic space, elements of the system, etc.). In OSeMOSYS, the group of sets include: years, fuels, technologies, emissions and modes of operation. As is going to be further explained, the sets are characterised through parameters. These subsections present the sets that compose the current version of OSeMOSYS-SL.  

2.2.1 Year
---------

This corresponds to the period of analysis. For OSeMOSYS-SL it is from 2015 to 2050. However, the data from 2015 to 2023 is set according to historical information. 

2.2.2 Fuels
---------
In the OSeMOSYS model fuels act as commodities, with their availability often split between the demand of several technologies. These are crutial in establishing limitations in the supply chain of Sierra Leone's power sector from the three main fuel sources of production, importation or renewable fuels available for use in energy generation within Sierra Leone.  

2.2.3 Technologies
---------
+---------------------------------------------------------------------------------------------------------------------+
| .. figure:: img/SL_RES_Diag.png                                                                                    |
|    :align:   center                                                                                                 |
|    :width:   500 px                                                                                                 |
+---------------------------------------------------------------------------------------------------------------------+
   *Figure 2.2.3: Reference Energy System for the technologies used in the Sierra Leone OSeMOSYS Model*

2.2.4 Emissions
---------

2.2.5 Mode of operation
---------

2.2.6 Region
---------

The model has a nationwide scope, therefore it only has one region: Sierra Leone (SL).
