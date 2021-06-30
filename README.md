This repository contains the datasets for our study "Stochastic mixed model sequencing with multiple stations using reinforcement learning and probability quantiles."

The dataset for the stochastic MMS problem is an extension of the dataset for the deterministic MMS problem by Boysen N, Kiel M, Scholl A (2011) "Sequencing mixed-model assembly lines to minimise the number of work overload situations," International Journal of Production Research 49, 4735-4760.

The repository is organized in three folders:

* main_analysis (Datasets of main analyses)

This folder contains ten subfolders Unique_Mut_0 to Unique_Mut_9. Each subfolder contains 216 files, one for each layout but with different a demand plan. Note that we generated ten demand plans for each layout.

* additional_stations (Analysis with additional stations on the assembly line)

This folder contains six subfolders Unique_Mut_0_Add_0_stations to Unique_Mut_0_Add_5_stations, which contain the problem instances with 0 to 6 additional stations on the assembly line.

* additional_models (Analysis with additional models in the demand plan)

This folder contains six subfolders Unique_Mut_0_Add_0_models to Unique_Mut_0_Add_5_models, which contain the problem instances with 0 to 6 additional models in the demand plan.
In addition, this folder contains another six folders Unique_Mut_0_Add_0_models_manhatten to Unique_Mut_0_Add_5_models_manhatten, which contain the simplified problem instances that are used by the reinforcement learning policies.

The syntax of a file describing a problem instance is as follows.

Line: content

1: number of models M <br>
2: demand plan for model m = 1,...,M <br>
3: number of stations K <br>
4: lengths of stations k=1,...,K <br>
5: cycle time <br>
6 -- end: processing times as a matrix of size K x M. The row index refers to the station and the column index refers to the model. 
