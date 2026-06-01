# Multivariate-time-series-forecasting

# Hyperparameter and other specifications:

* Sequence length = 96
* Batch size = 64
* Hidden layer = 64 (tested with 124 but showed overfit so changed to 64)
* Number of layers = 1 
* dropout = 0.3
* learning rate = 0.001
* epochs = 50 (The model didn't learn too much after 40 epochs in the original test)
* 80 - 20 train-test split
* Model : LSTM

# Features used:

* Export
* Import
* Generation
* National load
* System load
* Bhairahawa temperature 
* Bhairahawa specific humidity 
* Bhairahawa surface pressure
* Bhairahawa wind speed
* Biratnagar temperature
* Biratnagar specific humidity
* Biratnagar surface pressure
* Biratnagar wind speed
* Dhangadi temperature
* Dhangadi specific humidity
* Dhangadi surface pressure
* Dhangadi wind speed
* Kathmandu temperature
* Kathmandu specific humidity
* Kathmandu surface pressure
* Kathmandu wind speed
* Nepalgunj temperature
* Nepalgunj specific humidity
* Nepalgunj surface pressure
* Nepalgunj wind speed
* Pokhara temperature 
* Pokhara specific humidity
* Pokhara surface pressure
* Pokhara wind speed
* Birgunj temperature
* Birgunj specific humidity
* Birgunj surface pressure
* Birgunj wind speed

# TO DO

* Reduce the number of features. We have determined the importance and so on through which we remove precipitation but there's definitely more to do here.
* Clean out the data further. The data we received seems to have gaps that we have had to skip over.
* The parameters have been managed manually here. 
* Error distribution for the predicted data. 

# Outputs:

## The learning curves for training and validation:

![Learning curves](/images/Learning%20Curves.png)

## Complete forecast in the training set and for the first 96 data

![Forecast](/images/full%20test%20set%20and%20first%2096%20slots%20LSTM.png)

## Final forecast for 2026-01-31 (random selected date here) - MAE = 34.07 MW, MAPE = 2.29 %

![Final forecast for given date](/images/final%20complete%20forecast.png)