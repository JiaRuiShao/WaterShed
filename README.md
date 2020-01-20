
This research aims to predict how does precipitation, air temperature, snow melt, SWE, VMC these factors affect the downstream delivery of water, nutrients, carbon, and metals over seasonal to decadal timescales through the development and testing of scale-adaptive approaches. 
Besides the DryCreek project, which targets a smaller area of river with clean and enough historical data, there's another EastRiver Project which does not have as many data as the DryCreek one and the data also needed to be process. I worked on the EastRiver project first, processing the data, finding the optimal way to have the highest prediction. Then I moved on to the DryCreek project, which takes me a longer time and it's more well-structured and has fewer problems compared to the EastRiver one.


**DryCreek River**

I divided the LSTM model into two cases, one as a univariate time series model that only included previous discharge values in future prediction; the second was a multivariate DNN model that uses not only previous discharge values but also uses other relative features to predict future discharge. 

discharge preview:
![drycreek discharge](https://github.com/JiaRuiShao/WaterShed/blob/master/images/DryCreek_discharge.png?raw=true)

1. Univariate LSTM Model

[DryCreek Univariate LSTM Model Notebook](https://github.com/JiaRuiShao/WaterShed/blob/master/DryCreek/LSTM_DryCreek_Univariate_Predictive_Model.ipynb)

validation prediction under certain hyperparameters:
![uni val pred](https://github.com/JiaRuiShao/WaterShed/blob/master/images/univariate_validation_prediction.png?raw=true)

testing prediction under certain hyperparameters:
![uni test pred](https://github.com/JiaRuiShao/WaterShed/blob/master/images/univariate_testing_prediction.png?raw=true)

2. Multivariate LSTM Model

[DryCreek Multivariate LSTM Model Notebook](https://github.com/JiaRuiShao/WaterShed/blob/master/DryCreek/LSTM_DryCreek_Multivariate_Predictive_Model.ipynb)

still working on it to find the optimal hyperparameters...

**EastRiver River**

Data Process: [EastRiver Data Process](https://github.com/JiaRuiShao/WaterShed/blob/master/EastRiver/DataProcess_EastRiver.ipynb)

LSTM Model: [EastRiver LSTM Model Notebook](https://github.com/JiaRuiShao/WaterShed/blob/master/EastRiver/LSTM_EastRiver.ipynb)

**Reference**

https://github.com/JiaRuiShao/WaterShed/tree/master/Reference