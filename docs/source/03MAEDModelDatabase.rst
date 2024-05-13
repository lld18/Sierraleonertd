3. MAED model: Database
=======================================
This section presents a summary of the key socioeconomic data inputs for the MAED model used to predict energy demand in Sierra Leone, as well as key calculations used to allow this data to be used within the MAED model as well as outputting data formatted appropriately for use in the OSeMOSYS model. Along side the base-scenario established in this data are two other demand scenarios; a high GDP and population growth rate scenario, and a low GDP and population scenario outlined in sections 3.6 and 3.7. these are used to esablish high and low demand scenarios alongside the baseline scenario. 

3.1 Main Data Sources.
+++++++++
The table below summarises the main sources and assumptions recommended for the data used in the MAED study for Sierra Leone.

+----------------+------------+--------------------------+----------------------------------------------------------------------------+
| Category       | Source     | Data                     | Descriptions and assumption made                                           |
+================+============+==========================+============================================================================+
| Population     | World Bank | Sierra Leone Population  | Population of Sierra Leone in initial year of modelling.                   |
| parameters     | IMF        | (Millions)               |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | World      | Population Growth Rate   | Population growth rate in Sierra Leone. Assumed constant beyond            |
|                | Population | (%)                      | current projections.                                                       |
|                | Review     |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | Statistica | Urban Population (%)     | Portion of Sierra Leone's population reported to live in urban households  |
|                |            |                          | in initial year of modelling.                                              |
|                |            |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | SSL Reports| Persons per Urban        | Number of individuals per urban household in Sierra Leone.                 |
|                |            | Household (Capita)       | Assumed constant over the modelling period.                                |
|                |            |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | SSL Reports| Persons per Rural        | Number of individuals per rural household in Sierra Leone.                 |
|                |            | Household (Capita)       | Assumed constant over the modelling period                                 |
|                |            |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | World Bank | Potential Labour Force   | Portion of Sierra Leone's population with potential to participate         |
|                | Statistica | (%)                      | in the labour force. Assumed constant over the modelling period.           |
|                |            |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | World Bank | Participating Labour     | Portion of Sierra Leone's population participating in the labour force.    |
|                | Statistica | Force (%)                | Assumed constant over the modelling period.                                |
|                |            |                          |                                                                            |
+----------------+------------+--------------------------+----------------------------------------------------------------------------+
| GDP            | World Bank | GDP (US$ Millions)       | Sierra Leone's Gross Domestic Product (GDP) in the initial year of         |
| parameters     |            |                          | modelling.                                                                 |
|                |            |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | IMF        | GDP Growth Rate (%)      | The growth rate for Sierra Leone's GDP over the modelling period.          |
|                |            |                          | Assumed constant beyond current projections.                               |
|                |            |                          |                                                                            |
+----------------+------------+--------------------------+----------------------------------------------------------------------------+
| Sectoral       | SSL Report | Industry (Total)         | Total industrial share of Sierra Leone's GDP. Assumed constant over        |
| shares of GDP  |            |                          | the modelling period.                                                      |
|                |            |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | SSL Report | Industry (Agriculture)   | Agriculture's share of Sierra Leone's GDP. Assumed constant over the       |
|                |            |                          | modelling period.                                                          |
|                |            |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | SSL Report | Industry (Mining)        | Mining's share of Sierra Leone's GDP. Assumed constant over the modelling  |
|                |            |                          | period.                                                                    |
|                |            |                          |                                                                            |
|                |            |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | SSL Report | Services                 | Services share of Sierra Leone's GDP. Assumed constant over the modelling  |
|                |            |                          | period.                                                                    |
|                |            |                          |                                                                            |
|                |            |                          |                                                                            |
+----------------+------------+--------------------------+----------------------------------------------------------------------------+
| Baseline       | EDSA       | Industry (Total)         | Total energy consumption for Sierra Leone's Industrial sector.             |
| Sectoral       |            |                          |                                                                            |
| Energy         |            |                          |                                                                            |
| Consumption    |            |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | EDSA       | Industry (Agriculture)   | Energy consumption for Sierra Leone's Industry Agriculture sector,         |
|                |            |                          | assumed to equal 2% of Sierra Leones energy consumption.                   |
|                |            |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | EDSA       | Industry (Mining)        | Energy consumption for Sierra Leone's Industry Mining sector,              |
|                |            |                          | assumed to cover the share of Sierra Leone's Industrial sector             |
|                |            |                          | not accounted for by Sierra Leone's Agriculture sector.                    |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | EDSA       | Services                 | Energy consumption for Sierra Leone's Services sector.                     |
|                |            |                          |                                                                            |
|                |            |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | EDSA       | Household (Total)        | Energy consumption for all households in Sierra Leone.                     |
|                |            |                          |                                                                            |
|                |            |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | EDSA       | Household (Urban)        | Energy consumption for urban households in Sierra Leone. Assumed to equal  |
|                |            |                          | 95% of Sierra Leone's total household energy consumption.                  |
|                |            |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | EDSA       | Household (Rural)        | Energy consumption for urban households in Sierra Leone. Assumed to equal  |
|                |            |                          | the remaining 5% of Sierra Leone's total household energy consumption.     |
|                |            |                          |                                                                            |
+----------------+------------+--------------------------+----------------------------------------------------------------------------+
| Household      | World Bank | Urban Electrification    | Percentage of Sierra Leone's urban populations with access to electricity, |
| electrification| AEP data   |                          | electrification rates projected in line with Sierra Leone's Targets.       |
| rates (%)      | and        |                          |                                                                            |
|                | statistics |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | World Bank | Rural Electrification    | Percentage of Sierra Leone's rural populations with access to electricity, |
|                | AEP data   |                          | electrification rates projected in line with Sierra Leone's Targets.       |
|                | and        |                          |                                                                            |
|                | statistics |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | World Bank | National Electrification | Percentage of Sierra Leone's total population with access to electricity,  |
|                | AEP data   |                          | electrification rates projected in line with Sierra Leone's Targets.       |
|                | and        |                          |                                                                            |
|                | statistics |                          |                                                                            |
+----------------+------------+--------------------------+----------------------------------------------------------------------------+
| Sectoral energy| Calculated | Agriculture (MJ/US$)     | Agricultural productivity in terms of US$ per MJ of energy used.           |
| intensity per  | from IRP   |                          |                                                                            |
| annum          |            |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | Calculated | Mining (MJ/US$)          | Mining productivity in terms of US$ per MJ of energy used.                 |
|                | from IRP   |                          |                                                                            |
|                |            |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | Calculated | Services (MJ/US$)        | Services productivity in terms of US$ per MJ of energy used.               |
|                | from IRP   |                          |                                                                            |
|                |            |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | Calculated | Urban Household (MJ/US$) | Productivity of Urban Households in terms of US$ per MJ of energy used.    |
|                | from IRP   |                          |                                                                            |
|                |            |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | Calculated | Rural Household (MJ/US$) | Productivity of Rural Households in terms of US$ per MJ of energy used.    |
|                | from IRP   |                          |                                                                            |
|                |            |                          |                                                                            |
+----------------+------------+--------------------------+----------------------------------------------------------------------------+
| GDP Scenarios  | IMF        | Base GDP Growth Rate     | The annual growth rate for Sierra Leone's GDP over the modelling period,   |
|                |            |                          | assumed constant beyond available data.                                    |
|                |            |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | AfDB       | High GDP Growth Rate     | The annual growth rate for Sierra Leone's GDP over the modelling period,   |
|                | Review     |                          | linear projection to meet Sierra Leone's ambitions (currently 7% by 2035)  |   
|                |            |                          | and remaining constant beyond this horizon.                                |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | IMF        | Low GDP Growth Rate      | The annual growth rate for Sierra Leone's GDP over the modelling period,   |
|                |            |                          | assumed to remain at 2023 rates.                                           | 
|                |            |                          |                                                                            |
+----------------+------------+--------------------------+----------------------------------------------------------------------------+
| Population     | World      | Base Population Scenario | The annual growth rate for Sierra Leone's population, assumed to remain    |
| Scenarios      | Population |                          | constant beyond current projections.                                       |
|                | Review     |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                |            | High Population Scenario | The annual growth rate for Sierra Leone's population, assumed to equal     |
|                |            |                          | growth rates found in other related studies in Sierra Leone.               |
|                |            |                          |                                                                            |
+                +------------+--------------------------+----------------------------------------------------------------------------+
|                | World      | Low Population Scenario  | The annual growth rate for Sierra Leone's population, assumed to maintain  |
|                | Population |                          | annual changes growth rate in line with historic changes (-0.03% per year  | 
|                | Review     |                          | based on 2019-2021 growth rates)                                           |
+----------------+------------+--------------------------+----------------------------------------------------------------------------+

3.3. Summary of demographic parameters.
+++++++++
The table below summarises the key demographic parameters used as inputs for the MAED demand modelling in Sierra Leone. 

+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+
| Demographic         | Units      | Summary of Demographic Parameters                                                                |
| Variable            |            |                                                                                                  |
+                     +            +----------+----------+----------+----------+----------+----------+----------+----------+----------+
|                     |            | 2018     | 2019     | 2020     | 2021     | 2022     | 2023     | 2024     | 2025     | 2030     |
+=====================+============+==========+==========+==========+==========+==========+==========+==========+==========+==========+
| Population          | Millions   | 7.861    |          |          |          |          |          |          |          |          |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+
| Population          | %          |          | 2.13     | 2.09     | 2.06     | 2.06     | 2.06     | 2.06     | 2.06     | 2.07     |
| Growth Rate         |            |          |          |          |          |          |          |          |          |          |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+
| Urban               | %          |  42      | 42       | 43       | 43       | 44       | 44       | 45       | 45       | 50       |
| Population          |            |          |          |          |          |          |          |          |          |          |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+
| Persons per         | Capita     | 5        | 5        | 5        | 5        | 5        | 5        | 5        | 5        | 5        |
| Urban Household     |            |          |          |          |          |          |          |          |          |          |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+
| Persons per         | Capita     | 6        | 6        | 6        | 6        | 6        | 6        | 6        | 6        | 6        |
| Rural Household     |            |          |          |          |          |          |          |          |          |          |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+
| Potential           | %          | 72       | 72       | 72       | 72       | 72       | 72       | 72       | 72       | 72       |
| Labour Force        |            |          |          |          |          |          |          |          |          |          |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+
| Participating       | %          | 54       | 54       | 54       | 54       | 54       | 54       | 54       | 54       | 54       |
| Labour Force        |            |          |          |          |          |          |          |          |          |          |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+ 

3.2. Summary of economic parameters.
+++++++++
The table below summarises the key economic parameters used as inputs for the MAED demand modelling in Sierra Leone. 

+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+
| Economic            | Units      | Summary of Demographic Parameters                                                                |
| Variable            |            |                                                                                                  |
+                     +            +----------+----------+----------+----------+----------+----------+----------+----------+----------+
|                     |            | 2018     | 2019     | 2020     | 2021     | 2022     | 2023     | 2024     | 2025     | 2030     |
+=====================+============+==========+==========+==========+==========+==========+==========+==========+==========+==========+
| GDP                 | US$ Billion| 4.09     |          |          |          |          |          |          |          |          |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+
| GDP Growth          | %          |          | 5.25     | -2.00    | 4.10     | 3.98     | 2.75     | 4.74     | 5.19     | 4.60     |
| Rate                |            |          |          |          |          |          |          |          |          |          |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+
| Share of GDP                                                                                                                        |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+
| Industry (Total)    | %          | 63.3     | 63.3     | 63.3     | 63.3     | 63.3     | 63.3     | 63.3     | 63.3     | 63.3     |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+
| Industry            | %          | 57.4     | 57.4     | 57.4     | 57.4     | 57.4     | 57.4     | 57.4     | 57.4     | 57.4     |
| (Agriculture)       |            |          |          |          |          |          |          |          |          |          |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+
| Industry            | %          | 5.9      | 5.9      | 5.9      | 5.9      | 5.9      | 5.9      | 5.9      | 5.9      | 5.9      |
| (Mining)            |            |          |          |          |          |          |          |          |          |          |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+
| Services            | %          | 36.7     | 36.7     | 36.7     | 36.7     | 36.7     | 36.7     | 36.7     | 36.7     | 36.7     |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+ 
| Total               | %          | 100      | 100      | 100      | 100      | 100      | 100      | 100      | 100      | 100      |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+ 

3.3. Summary of baseline sectoral energy consumption.
+++++++++
The table below summarises estimates for the energy demand within each sector modelled in Sierra Leone over a historic baseline period.

+-------------------------+-----------------+-----------------+-----------------+-----------------+-----------------+-----------------+
| Sector                  | Total Energy Consumtion (GWh)                                                                             |
|                         |                                                                                                           |
+                         +-----------------+-----------------+-----------------+-----------------+-----------------+-----------------+
|                         | 2018            | 2019            | 2020            | 2021            | 2022            | 2023            | 
+=========================+=================+=================+=================+=================+=================+=================+
| Industrial (Total)      | 42.50           | 70.00           | 68.89           | 68.89           | 82.78           | 96.94           | 
+-------------------------+-----------------+-----------------+-----------------+-----------------+-----------------+-----------------+
| Industrial (Agriculture)| 3.36            | 5.38            | 5.29            | 5.29            | 6.38            | 7.51            | 
+-------------------------+-----------------+-----------------+-----------------+-----------------+-----------------+-----------------+
| Industrial (Mining)     | 39.14           | 64.71           | 63.59           | 63.59           | 76.39           | 89.43           | 
+-------------------------+-----------------+-----------------+-----------------+-----------------+-----------------+-----------------+
| Services                | 49.72           | 81.39           | 68.89           | 68.89           | 82.78           | 96.94           | 
+-------------------------+-----------------+-----------------+-----------------+-----------------+-----------------+-----------------+
|Household (Total)        | 75.83           | 124.44          | 122.50          | 122.50          | 147.22          | 172.50          | 
+-------------------------+-----------------+-----------------+-----------------+-----------------+-----------------+-----------------+
|Household (Urban)        | 72.04           | 118.22          | 116.38          | 116.38          | 139.86          | 163.88          | 
+-------------------------+-----------------+-----------------+-----------------+-----------------+-----------------+-----------------+
|Household (Rural)        | 3.79            | 6.22            | 6.12            | 6.12            | 7.36            | 8.62            | 
+-------------------------+-----------------+-----------------+-----------------+-----------------+-----------------+-----------------+
|Total                    | 168.06          | 268.89          | 264.72          | 264.72          | 319.17          | 375.56          | 
+-------------------------+-----------------+-----------------+-----------------+-----------------+-----------------+-----------------+

3.4. Summary of electrification rates in Sierra Leone over baseline years.
+++++++++
This table summarises electrification rates at both a national and rural and urban levels within Sierra Leone across key years.

+-------------+-----------+-----------+-----------+-----------+-----------+-----------+-----------+-----------+-----------+-----------+
| Scale       | Household Electrification Rate (%)                                                                                    |
|             |                                                                                                                       |
+             +-----------+-----------+-----------+-----------+-----------+-----------+-----------+-----------+-----------+-----------+
|             | 2018      | 2019      | 2020      | 2021      | 2022      | 2023      | 2025      | 2030      | 2040      | 2050      |
+=============+===========+===========+===========+===========+===========+===========+===========+===========+===========+===========+
| Urban       | 53.20     | 51.40     | 55.00     | 57.00     | 57.00     | 57.00     | 61.82     | 73.87     | 98.00     | 100.00    |
+-------------+-----------+-----------+-----------+-----------+-----------+-----------+-----------+-----------+-----------+-----------+
| Rural       | 6.40      | 4.70      | 4.70      | 4.90      | 4.90      | 4.90      | 10.90     | 26.00     | 56.00     | 86.00     |
+-------------+-----------+-----------+-----------+-----------+-----------+-----------+-----------+-----------+-----------+-----------+

3.5. Summary of Sierra Leone's sectoral energy intensities per annum
+++++++++
This table summarises the energy intensities of each of the outlined sectors in Sierra Leone.

+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+
| Sector              | Units      | Energy Intensity                                                                                 |
|                     |            |                                                                                                  |
+                     +            +----------+----------+----------+----------+----------+----------+----------+----------+----------+
|                     |            | 2018     | 2019     | 2020     | 2021     | 2022     | 2023     | 2030     | 2040     | 2050     |
+=====================+============+==========+==========+==========+==========+==========+==========+==========+==========+==========+
| Agriculture         | MJ/US$     | 0.0056   | 0.0083   | 0.0074   | 0.0075   | 0.0089   | 0.0088   | 0.0104   | 0.0133   | 0.0170   |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+
| Mining              | MJ/US$     | 0.3643   | 0.5415   | 0.4860   | 0.4868   | 0.5813   | 0.5720   | 0.8512   | 1.4149   | 2.2002   |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+
| Services            | MJ/US$     | 0.2332   | 0.3456   | 0.3107   | 0.3127   | 0.3723   | 0.3664   | 0.3622   | 0.3404   | 0.3024   |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+
| Urban Household     | MJ/dw/yr   | 4856.4   | 7658.5   | 6032.0   | 5987.0   | 7093.1   | 7026.1   | 7463.4   | 9704.6   | 15252    |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+
| Rural Household     | MJ/dw/yr   | 2124.7   | 4408.2   | 3715.1   | 3665.5   | 4342.7   | 4301.7   | 2356.1   | 4244.5   | 7600.9   |
+---------------------+------------+----------+----------+----------+----------+----------+----------+----------+----------+----------+

3.6. GDP Growth Scenario Variables
+++++++++
Energy demand scenarios were stablished for High and Low cases above and below the base scenario. The difference between these scenarios are driven in part by differences in the growth rates projected for Sierra Leone's GDP, with lower demand scenarios under more concervitive estimates of the bounds of Sierra Leone's GDP growth, whilst higher demand scenarios are associated with higher GDP growth scenarios. This table summarises the differences in GDP growth rates under these high and low energy demand scenarios.

+-------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------+
| Scenario    | GDP Growth Rate (%)                                                                                                   |
|             |                                                                                                                       |
+             +--------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------+
|             | 2023         | 2024         | 2025         | 2030         | 2035         | 2040         | 2045         | 2050         | 
+=============+==============+==============+==============+==============+==============+==============+==============+==============+
| Base        | 2.75         | 4.74         | 5.19         | 4.60         | 4.60         | 4.60         | 4.60         | 4.60         |
+-------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------+
| High        | 2.75         | 4.74         | 5.19         | 7.00         | 7.00         | 7.00         | 7.00         | 7.00         |
+-------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------+
| Low         | 2.75         | 2.75         | 2.75         | 2.75         | 2.75         | 2.75         | 2.75         | 2.75         |
+-------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------+

3.7. Population Growth Scenario Variables
+++++++++
Energy demand scenarios are also driven by differences in estimates of Sierra Leone's population growth. Higher growth estimates are reflected in the higher demand scenario, whilst more conservative growth scenarios result in the lower energy demand scenario. This table summarises the differences in population growth rates under these high and low energy demand scenarios.

+--------------+----------------+----------------+----------------+----------------+----------------+----------------+----------------+
| Scenario     | Population Growth Rate (%)                                                                                           |
|              |                                                                                                                      |
+              +----------------+----------------+----------------+----------------+----------------+----------------+----------------+
|              | 2023           | 2025           | 2030           | 2035           | 2040           | 2045           | 2050           | 
+==============+================+================+================+================+================+================+================+
| Base         | 2.06           | 2.06           | 2.06           | 2.06           | 2.06           | 2.06           | 2.06           |
+--------------+----------------+----------------+----------------+----------------+----------------+----------------+----------------+
| High         | 2.06           | 2.54           | 2.54           | 2.54           | 2.54           | 2.54           | 2.54           |
+--------------+----------------+----------------+----------------+----------------+----------------+----------------+----------------+
| Low          | 2.05           | 2.00           | 1.85           | 1.70           | 1.55           | 1.40           | 1.25           |
+--------------+----------------+----------------+----------------+----------------+----------------+----------------+----------------+



