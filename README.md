# Stock Market Forecasting using LSTM and GRU
## About the Project
This project involves predicting the prices of various stocks (considered **APPL** and **AMD** stocks) using previous stock prices data. Used deep learning models - **LSTM**(Long Short Term Memory) and **GRU**(Gated Recurrent Unit), both of which are variations of **RNN**(Recurrent Neural Network).

## Usage
Go to the project directory and install the dependencies using the command
```
pip install -r requirements.txt
```
To run the code, execute the following command.
```
python run.py
```

## Dataset
The dataset used in this project was downloaded from **Yahoo Finance**. The stock prices of APPL was downloaded for two years (2022-2023) and stock prices of AMD was downloaded for about approximately seven years (2017-2023).

## Methodology
The files `datavis.py` and `dataprep.py` are used for visualizing the stock prices using various plots and preparing the stock prices data for the purpose of training the model. 
The stock prices are normalized using the **MinMaxScaler** and sequences of the prices are made for the purpose of training.

The models **LSTM** and **GRU** are defined in the file `model.py`. 
The models are then trained and the results are evaluated based on various metrics like **RMSE**, **MSE**, **MAE**, **R<sup>2</sup>** in the `train.py` file. 

Various graphs are also plotted to understand the results better. Graphs of results for AAPL stock can be found in the `results_graphs` folder. 
The **actual vs predicted price values** of the test data are stored in the csv files.

It was observed that the GRU model performed better in capturing the short term changes in the stock prices compared to LSTM.

