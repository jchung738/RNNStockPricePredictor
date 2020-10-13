# RNNStockPricePredictor
This is a Google Colab notebook that uses transformed transactional trading data for $AAPL to make predictions on the direction of the stock price. The data is transformed into 5 minute bins with features such as price high, low, and mean, volume, time of day, and day of week. The dataset itself is not included as it is expensive to procure and is not required to demonstrate the techniques in the Jupyter notebook. For making predictions I used a Recurrent Neural Network that has LSTM, Dropout, and Dense layers using Keras frontend and Tensorflow backend. In order to simulate the performance of the model in a streaming context, we use walk-forward validation to train the neural network over time, incrementally changing weights over the dataset. At the end of the notebook there is a nice thought experiment of potential "profit" if trades were executed according to the model's predictions. Of course this is not how this would work in a real firm and the "profit" is more determined by the overall performance of AAPL over the last 10 years rather than the model's performance. 
