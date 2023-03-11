# Stock-Price-Prediction-Visualization
Stock price prediction of State Bank of India and visualization of SBI and Reliance Industries stock
<h1> Overview </h1>
<p> This code is a Machine Learning (ML) program that predicts the stock prices of two Indian companies, State Bank of India (SBIN) and Reliance Industries Limited (RELIANCE). The program uses historical data from Yahoo Finance to train a Long Short-Term Memory (LSTM) model to predict future stock prices. The program begins by importing the required libraries, including Pandas, Numpy, Matplotlib, Seaborn, and the Yahoo Finance API. Next, it downloads one year of historical data for SBIN and RELIANCE and plots the Adjusted Close price of the stocks. The program then selects the closing price of SBIN for further analysis, scales the data, and creates a training data set using a sliding window technique. The LSTM model is constructed, compiled, and trained using the training data set. The program then creates a testing data set, makes predictions using the trained model, and calculates the Root Mean Squared Error (RMSE) between the predicted values and actual values. Overall, the program provides an example of using an LSTM model to predict stock prices and can be easily adapted to other companies and timeframes.</p>

<h1> Requirements </h1>
<ul> <h3> Python version </h3> </ul> 
  <li> Python 3.7 or above </li>
