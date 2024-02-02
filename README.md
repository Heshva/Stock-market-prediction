# Stock-market-prediction

	The Stock Prediction is an advanced stock prediction system designed to forecast the performance of stocks over a specific duration. 
	Using machine learning algorithms and historical stock data, the system analyzes patterns, trends, and market indicators to generate accurate predictions.


	In the following Code I’ve done the following things:

•	Libraries I’ve import

o	yfinance 
o	from TensorFlow, keras
o	import NumPy 
o	from sklearn.preprocessing, MinMaxScaler
o	from sklearn.metrics ,mean_squared_error
o	from matplotlib, pyplot 

•	Asks the user to input a stock symbol. (Ex., i want to import data of TESLA then i'll write stock symbol TSLA ) 

•	Downloads historical stock data for the specified stock symbol from Yahoo Finance, saves it to a CSV file, and prints the downloaded data.

•	Normalizes the "Close" price data using Min-Max scaling.

•	Creates sequences of input (X) and output (y) data for training a Long Short-Term Memory (LSTM) model. The sequence length is set to 10.

•	Splits the data into training and testing sets, with 80% of the data used for training and 20% for testing.

•	Defines an LSTM model with one LSTM layer with 50 units and a ReLU activation function, followed by a dense output layer.

•	Compiles the model using the Adam optimizer and mean squared error as the loss function.

•	Trains the model on the training data for 20 epochs with a batch size of 32.

•	Predicts the stock price for the next day based on the last sequence from the test data.

•	Inverse transforms the scaled prediction to obtain the predicted price in the original scale.

•	Calculates and prints the mean squared error between the real and predicted stock prices.

•	Visualizes the real and predicted stock prices using a line plot.

