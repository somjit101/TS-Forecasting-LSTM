# Time Series Forecasting with LSTMs
A detailed study on the use of Long Short Term Memory (LSTM) units for time series forecasting with climate data.

## Problem Statement

Here the problem statement is to predict future, unknown values in a time series depicting the readings of various atmospheric measurements comprising the weather of a place like **temperature**, **pressure**, **pressure**, **wind velocity**, **wind direction** etc. given historical data readings of the same. 

We have implemented a simple moving average forecasting model as a reference model to demonstrate how the LSTM-based forecasting models perform with respect to the reference model. </br>
It is safe to assume that there is a significant collinearity among all the parameters, i.e. the readings have an underlying relationship among them, i.e. they influence each other and not independent to each other. We will be examining this aspect by comparing the performances of both univariate and multivariate LSTM-based prediction models. 

## Dataset

The [Max-Planck Institute Weather Data](https://www.bgc-jena.mpg.de/wetter/) is regularly maintained for numerous applications in scientific research and reporting. There are numerous atmospheric measurements which are updated in real time and can be used for our case study. </br>
The specific dataset we have used here captures weather data from the year 2009 to 2016 and can be downloaded [here](https://storage.googleapis.com/tensorflow/tf-keras-datasets/jena_climate_2009_2016.csv.zip).

### Reference

[Tensorflow Article on Time Series Forecasting](https://www.tensorflow.org/tutorials/structured_data/time_series)
