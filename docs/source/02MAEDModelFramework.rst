2. MAED model: framework 
=======================================
This documentation outlines the methodology used to generate the Model for Analysis of Energy Demand (MAED) for use in the OSeMOSYS modelling approach. MAED is a demand model developed by the IAEA that projects future national and sectoral energy demands based on medium and long-term socioeconomic, technological and demographic projections. Therefore this documentation aims to outline the key assumptions and sources for data inputs for use in this model, as well as key calculations. The framework of this model is outlined below. 

2.1. MAED Model Structure
+++++++++

 .. figure:: img/SL_MAED_Diag.png
    :align:   center
    :width:   750 px

   *Figure 2.1: Simplified summary of the process of MAED projecting future demand*

2.2. MAED Sets
+++++++++

Demand for Sierra Leone was calculated using the open-source IAEA MAED model. This requires a number of socioeconomic parameters to project energy demand in key sectors. A summary of these sets is outlined below.

2.2.1 Population
---------

The population for Sierra Leone reported in the first year of modelling which is currently set to 2018 for use in the MAED model and must be reported in millions of individuals. This provides the baseline from which MAED will project future population growth.

2.2.2 Population Growth Rate
---------
The annualised population growth rate for Sierra Leone's population over the modelling period of 2018-2050 based on the available data. This is used to assess the growth of Sierra Leone's existing GDP under projected scenarios, and can be adjusted to reflect higher or lower population growth scenarios in conjunction with high and low GDP growth scenarios to develop corresponding energy demand scenarios. 

2.2.3 Urban Population Share
---------
The share of Sierra Leone's population living in Urban Households. This projects potential changes in the share of Sierra Leone's population living in urban areas compared to those living in rural areas based on available data. 

2.2.4 Persons per Urban Household
---------
The average number of occupants per urban household in Sierra Leone. This is used to scale energy demand based on Sierra Leone's urban population and urban household energy demand parameters. 

2.2.5 Persons per Rural Household
---------
The average number of occupants per rural household in Sierra Leone. This is used to scale energy demand based on Sierra Leone's rural population and rural household energy demand parameters. 

2.2.6 Potential Labour Force Share
---------
This represents the percentage of Sierra Leone's population that has the potential to contribute to the national labour force. This is currently assumed to remain constant over the modelling period 2018-2050 in lieu of sufficient data.

2.2.7 Participating Labour Fource Share
---------
The percentage of Sierra Leone's population that is reported to actively participate and contribute to the national labour force. This is currently assumed to remain constant over the modelling period 2018-2050 in lieu of sufficient data.

2.2.8 GDP (USD Millions)
---------
The GDP for Sierra Leone reported in the first year of modelling which is currently set to 2018 for use in the MAED model and must be reported in Billion US Dollars. This provides the baseline from which MAED will project future GDP growth.

2.2.9 GDP Growth Rate
---------
The annualised GDP growth rate for Sierra Leone's GDP over the modelling period of 2018-2050 based on the available data. This is used to assess the growth of Sierra Leone's existing population under projected scenarios, and can be adjusted to reflect higher or lower GDP growth scenarios in conjunction with high and low population growth scenarios to develop corresponding energy demand scenarios. 

2.2.10 Sectoral Shares of GDP
---------
The percentile share that each sector contributes to Sierra Leone's net GDP.

2.2.11 Electrification Rates
---------
The percentage elecrtrification rates for Rural and Urban households in Sierra Leone, as well as the overall national electrification rate. 

2.2.12 Energy Balance
---------
The total energy demand for each sector over the baseline period reported in Petajoules (PJ). (The conversion from PJ to GWh is 1PJ = 277.777˙). 
