5. OSeMOSYS model: Database
=======================================
This section presents the main databases explored for building OSeMOSYS-SL, and the way the information was processed in order to introduce it to the model. 

3.1 Main data sources
+++++++++

3.1.1 Energy balance of Sierra Leone
---------

The energy balance is the most important source of data for the energy model of OSeMOSYS-SL. 


3.1.2 Other key databases 
---------

In the model, all fuels and technologies are incorporated to OSeMOSYS taking into account other sets, such as temporary divisions and emission, as well as the parameters. The latter are classified, among others, into costs, activity levels and infrastructure capacities. The establishment of these parameters was done after processing and reviewing the available national energy data. Table 3.1 summarizes the main souces of data for OSeMOSYS-CR. 

*Table 3.1.2: Main data sources used in OSeMOSYS-CR.*

.. table:: 
   :align:   center
+--------------+------------+--------------------------+------------------------------------------------------------------------------+
| Category     | Source     | Data                     | Descriptions and assumption made                                             |
+==============+============+==========================+==============================================================================+
| Energy       |            | Energy balance           |                                                                              |
| System       |            |                          |                                                                              |
+--------------+------------+--------------------------+------------------------------------------------------------------------------+
| Demand       |            | Final energy             |                                                                              |
|              |            |                          |                                                                              |
+              +------------+--------------------------+------------------------------------------------------------------------------+
|              |            | Transport                |                                                                              |
|              |            | (passengers and cargo)   |                                                                              |
|              |            |                          |                                                                              |
|              |            |                          |                                                                              |
+--------------+------------+--------------------------+------------------------------------------------------------------------------+
|Electricity   | IEA        | Capital and fixed costs  | Based on national data. The costs were assumed constant in the whole period, |
|technologies  |            |                          | except for solar and wind systems, which decrease according to international |
|              |            |                          |                                                                              |
+              +------------+--------------------------+------------------------------------------------------------------------------+
|              |            | Capacity and activity    | Based on the operational performance registered by the National Energy       |
|              |            |                          | Control Centre. Operational life is according to national plans.             |
+--------------+------------+--------------------------+------------------------------------------------------------------------------+
|Transport     |            | Capital and fixed costs  | Based on the Ministry of Finance (Hacienda) database. We assumed that cost of|
|technologies  |            |                          | electric vehicles decreases (Bloomberg). For cargo transport, we review cost |
|              |            |                          | of companies like Nicola and Tesla.                                          |
+              +------------+--------------------------+------------------------------------------------------------------------------+
|              |            | Capacity and activity    | Based on the performance register by national surveys, concession for public |
|              |            |                          | transport and the annual Vehicle technical review (RITEVE). Operational life |
|              |            |                          | is according to manufacturers and the residual capacity decreases linearly   | 
|              |            |                          | and proportionally with this value.                                          |
+--------------+------------+--------------------------+------------------------------------------------------------------------------+
|Fuel prices   | IEA        | Fossil Fuels and Biofuels| Based on current tariffs and projection uses in national plans. It considers |
|              |            |                          | international prices and the tariff given by the regulator in Costa Rica     |
|              |            |                          | (ARESEP) and trend provide by international Energy Agency (IEA).             |
+              +------------+--------------------------+------------------------------------------------------------------------------+
|              |            | Electricity              | Base of the average of national tariffs and projections.                     |
|              |            |                          |                                                                              |
+              +------------+--------------------------+------------------------------------------------------------------------------+
|              |            | Biomass                  |  Not included. It is produced and consumed locally.                          |
+              +------------+--------------------------+------------------------------------------------------------------------------+
|              |            | Hydrogen                 | Based on data published by ETSAP.                                            |
+--------------+------------+--------------------------+------------------------------------------------------------------------------+
|Infrastrucure |            | Plants and power grid    | Based on Transmission and generation national plans. It assumes losses of 4% |
|              |            |                          | from the bulk transmission system and 6% for distribution. Charging          |
|              |            |                          | infrastructure is not included.                                              |
+              +------------+--------------------------+------------------------------------------------------------------------------+
|              |            | Pipeline and road        | Based on national reports, we consider the current infraestructure does not  |
|              |            | distribution             | grow (gasoline and diesel). It includes new infrastructure for LPG. The model|
|              |            |                          |                                                                              |
+              +------------+--------------------------+------------------------------------------------------------------------------+
|              |            | Hydrogen                 |                                                                              |
+--------------+------------+--------------------------+------------------------------------------------------------------------------+
| Sustainable  |            | Urban plans and mobility |                                                                              |
| mobility     |            |                          |                                                                              |
|              |            |                          |                                                                              |
+--------------+------------+--------------------------+------------------------------------------------------------------------------+
| Cargo        |            | Electric cargo train and |                                                                              |
| transport    |            | Logistic                 |                                                                              |
|              |            |                          |                                                                              |
+--------------+------------+--------------------------+------------------------------------------------------------------------------+
| Emissions    | IPCC       |  Factors                 | Based on the IPCC and the national GHG inventory.                            |
+--------------+------------+--------------------------+------------------------------------------------------------------------------+
| Co-benefits  |            | Coefficients             |                                                                              |
|              |            |                          |                                                                              |
+--------------+------------+--------------------------+------------------------------------------------------------------------------+


3.1.3 Summary of Sierra Leone power plant capital costs
---------
Capital costs for power projects within Sierra Leone were collected from sources reported in Table 3.1.2.These costs reflect the cost associated with the construction of these power plants in order to meet the national demands predicted by OSeMOSYS. This is assumed to remain constant for many technologies, however for rapidly developing technologies such as solar, learning curves account for decreases in the technological cost associated with increased uptake of solar. these costs are summarised across key years in the table below. 

.. table:: 
   :align:   center
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Power Plant Type                 | Summary technology capital costs ($/kW)                               |
|                                  |                                                                       |
+                                  +-----------+-----------+-----------+-----------+-----------+-----------+
|                                  |    2021   |    2022   |    2023   |    2030   |    2040   |    2050   |
+==================================+===========+===========+===========+===========+===========+===========+
| Biomass Power Plant              |   2500    |   2500    |   2500    |   2500    |   2500    |   2500    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Coal Power Plant                 |   3739    |   3739    |   3739    |   3739    |   3739    |   3739    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| LFO (Diesel) Power Plant         |    795    |    795    |    795    |    795    |    795    |    795    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| HFO Power Plant                  |   1086    |   1086    |   1086    |   1086    |   1086    |   1086    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Gas Plant (CCGT)                 |   1014    |   1014    |   1014    |   1014    |   1014    |   1014    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Gas Plant (SCGT)                 |    795    |    795    |    795    |    795    |    795    |    795    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Karpowership                     |   0.0001  |   0.0001  |   0.0001  |   0.0001  |   0.0001  |   0.0001  |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Bumbuna Hydropower               |   3000    |   3000    |   3000    |   3000    |   3000    |   3000    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Betmai Hydropower                |   2500    |   2500    |   2500    |   2500    |   2500    |   2500    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Bekongor Hydropower              |   3000    |   3000    |   3000    |   3000    |   3000    |   3000    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Singimi Hydropower               |   2500    |   2500    |   2500    |   2500    |   2500    |   2500    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Bumbuna I 50 MW                  |   1500    |   1500    |   1500    |   1500    |   1500    |   1500    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Bumbuna I 88 MW                  |   9375    |   9375    |   9375    |   9375    |   9375    |   9375    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Bumbuna II 55MW                  |   6818    |   6818    |   6818    |   6818    |   6818    |   6818    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Hydropower with Reservoir        |   3000    |   3000    |   3000    |   3000    |   3000    |   3000    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Large Hydro (>100MW)             |   3000    |   3000    |   3000    |   3000    |   3000    |   3000    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Medium Hydro (10-100MW)          |   2500    |   2500    |   2500    |   2500    |   2500    |   2500    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Small Hydro (<10MW)              |   3000    |   3000    |   3000    |   3000    |   3000    |   3000    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Mini-Grid (Solar) with Storage   |   3500    |   3274    |   3048    |   2332    |   1895    |   1895    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Mini-Grid (Diesel)               |   1086    |   1086    |   1086    |   1086    |   1086    |   1086    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Mini-Grid (Hydro)                |   4000    |   4000    |   4000    |   4000    |   4000    |   4000    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Mini-Grid (Solar Hybrid)         |   3500    |   3274    |   3048    |   2332    |   1895    |   1895    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Mini-Grid (Diesel Hybrid)        |   1086    |   1086    |   1086    |   1086    |   1086    |   1086    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Solar PV (Utility)               |   829     |   818     |   808     |   740     |   657     |   657     |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Solar PV (Utility with Storage)  |   1958    |   1829    |   1700    |   1220    |   992     |    927    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Floating Solar PV (Utility)      |   1169    |   1169    |   1169    |   1169    |   1169    |   1169    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Off-Grid Generation (Diesel)     |   1086    |   1086    |   1086    |   1086    |   1086    |   1086    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Off-Grid Generation (Solar PV)   |   4139    |   3958    |   3777    |   2700    |   2091    |   2091    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Off-Grid Generation (Hydro)      |   3000    |   3000    |   3000    |   3000    |   3000    |   3000    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Crude Oil Refinery               |   24.1    |   24.1    |   24.1    |   24.1    |   24.1    |   24.1    |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Electricity Imports (Guinea)     |  0.0001   |  0.0001   |  0.0001   |  0.0001   |  0.0001   |  0.0001   |
+----------------------------------+-----------+-----------+-----------+-----------+-----------+-----------+
| Electricity Imports (CLSG)       |  0.0001   |  0.0001   |  0.0001   |  0.0001   |  0.0001   |  0.0001   |
