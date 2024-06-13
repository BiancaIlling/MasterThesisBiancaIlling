# MasterThesisBiancaIlling
Code and Data of my Master Thesis "The Impact of the Proliferation of Dynamic Household Tariffs on Grid Overloading".

In the "master" branch, all data, results, and code are stored. To get started, download the following data files:
- '1920 Final Data w. Additional Features HH Hourly Agg.pkl'
- '1920 Final Data w. Additional Features HP Hourly Agg.pkl'
- 'Gro_handelspreise_201901010000_202001312359_Stunde.csv'
- 'Dataset 1_EV charging reports.csv'
With these files, you can start by executing the notebook '0.Preprocessing'. Alternatively, you can also download the already preprocessed data.

Afterwards, the three different optimizations can be executed depending on which grid charge model should be used.
- 1.1 is the optimization in case of volumetric grid charges
- 1.2 in case of volumetric grid charges and additional peak price grid charges
- 1.3 implements the optiization for the three-level segmented grid charges.
With the results of the optimization, the power flow within the reference network "Kerber Dorfnetz" can be calculated to obtain the transformer load, line loading, and voltages for every time step, by using notebook '2.PowerFlowCalculation'. Already calculated results can also be used, which are found in the folder "results".

Using notebook 3.1, first insights into shifted household consumption patterns and the impact on the distribution grid are evaluated using dynamic or flat energy prices with volumetric grid charges for all households. Notebook 3.2 provides an overview of all different scenarios of grid charges combined with different shares of households using dynamic electricity tariffs, as well as a comparison of household costs in every scenario. In notebook 3.3, the sensitivity analysis on different interval lengths used for shifting the heat pump is conducted.
