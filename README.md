# Timeseries Classification challenge AN2DL Politecnico di Milano 2022
This is the model that I used in the [Timeseries Classification Challenge](https://codalab.lisn.upsaclay.fr/competitions/9056#results) of the course "Artificial Neural Networks and Deep Learning" course held at Politecnico di Milano in 2022.

The challenge consisted on the classification of 12 different time-structure data with the dimension of `(87444, 6)`. The model me and my team developed uses the 1D CNN (TCN).

We ended up acheiving an **accuracy of 75%**, you can check the results [here](https://codalab.lisn.upsaclay.fr/competitions/9056#results).

## Models details
For more details about the model check the [Report](report/Report.pdf). Briefly, we used the following techniques:
1. Building our own sequences using a sliding window function with a window size of 36 and a stride of 12.
2. Applying RobustScaler which helped in handling the possible presence of outliers
3. We chose to use simple TCN model with few number of layers, we performed a hyperparameters search to define the structure of the network. 
