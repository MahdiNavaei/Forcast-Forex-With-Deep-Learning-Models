# Forcast-Forex-With-Deep-Learning-Models

This code retrieves financial data from Tiingo API and trains a SimpleRNN neural network model on the EURJPY currency pair's historical data to make predictions.

The following libraries are used in this code:

* pandas
* numpy
* matplotlib
* seaborn
* requests
* datetime
* scipy
* pylab
* statsmodels
* sklearn
* keras
* tensorflow


After importing the required libraries, the code sets the necessary variables such as the API key, start and end dates for the data retrieval, the financial asset's ticker symbol, and the interval for resampling. The retrieved data is saved in an Excel file using the pandas library.

The data is then preprocessed, which includes converting the 'date' column to a datetime format, dropping the 'ticker' column, setting the 'date' column as the index, and plotting the probability distribution and ACF plots of the 'high' column.

The data is then split into training and testing sets, and MinMax scaling is applied to both input and output data. The RNN model is then defined, compiled, and trained using the training set. Finally, the model's performance is evaluated using the testing set, and the training history is saved for further analysis.
