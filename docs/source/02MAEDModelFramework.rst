2. MAED model: framework 
=======================================
This documentation outlines the methodology used to generate the Model for Analysis of Energy Demand (MAED) for use in the OSeMOSYS modelling approach. MAED is a demand model developed by the IAEA that projects future national and sectoral energy demands based on medium and long-term socioeconomic, technological and demographic projections. Therefore this documentation aims to outline the key assumptions and sources for data inputs for use in this model, as well as key calculations. The framework of this model is outlined below. 

2.1. MAED Model Structure
+++++++++
+---------------------------------------------------------------------------------------------------------------------+
| .. figure:: img/SL_MAED_Diag.png                                                                                    |
|    :align:   center                                                                                                 |
|    :width:   750 px                                                                                                 |
+---------------------------------------------------------------------------------------------------------------------+
   *Figure 2.1: Simplified summary of the process of MAED projecting future demand*

2.2. MAED Sets
+++++++++

Demand for Sierra Leone was calculated using the open-source IAEA MAED model. This requires a number of socioeconomic parameters to project energy demand in key sectors. A summary of these sets is outlined below.

2.2.1 Population
---------
This represents the population for Sierra Leone in millions  for the initial year of modelling which in this initial MAED model is set to 2018. This provides the baseline from with MAED will project future population growth.

2.2.2 Population Growth Rate
---------
The annualised population growth rate for Sierra Leone's population over the modelling period based on available data.

2.2.3 Urban Population Share
---------
The share of Sierra Leone's population living in Urban Households.

2.2.4 Persons per Urban Household
---------
The average number of occupants per urban household in Sierra Leone.

2.2.5 Persons per Rural Household
---------
The average number of occupants per rural household in Sierra Leone. 

2.2.6 Potential Labour Force Share
---------
The percentage of Sierra Leone's population that has the potential to contribute to the national labour force. 

2.2.7 Participating Labour Fource Share
---------
The percentage of Sierra Leone;s population that participates and actively contributes to the national labour force. 

2.2.8 GDP (USD Millions)
---------
The GDP for Sierra Leone reported in the first year of modelling, reported in Billion US Dollars.

2.2.9 GDP Growth Rate
---------
Annualised estimates of the growth rate of Sierra Leone's GDP over the modelling period based on available data.

2.2.10 Sectoral Shares of GDP
---------
The percentile share that each sector contributes to Sierra Leone's net GDP.

2.2.11 Electrification Rates
---------
The percentage elecrtrification rates for Rural and Urban households in Sierra Leone, as well as the overall national electrification rate. 

2.2.12 Energy Balance
---------
The total energy demand for each sector over the baseline period reported in Petajoules (PJ). (The conversion from PJ to GWh is 1PJ = 277.777˙). 
