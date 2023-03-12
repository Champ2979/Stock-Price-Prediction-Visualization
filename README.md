# Stock-Price-Prediction using (LSTM).
Stock price prediction of State Bank of India and visualization of SBI and Reliance Industries stock
<h1> Overview </h1>
<p> This code is a Machine Learning (ML) program that predicts the stock prices of an Indian company name State Bank of India (SBIN) and visualization of SBI and Reliance Industries Limited (RELIANCE). The program uses historical data from Yahoo Finance to train a Long Short-Term Memory (LSTM) model to predict future stock prices. The program begins by importing the required libraries, including Pandas, Numpy, Matplotlib, Seaborn, and the Yahoo Finance API. Next, it downloads one year of historical data for SBIN and RELIANCE and plots the Adjusted Close price of the stocks. The program then selects the closing price of SBIN for further analysis, scales the data, and creates a training data set using a sliding window technique. The LSTM model is constructed, compiled, and trained using the training data set. The program then creates a testing data set, makes predictions using the trained model, and calculates the Root Mean Squared Error (RMSE) between the predicted values and actual values. Overall, the program provides an example of using an LSTM model to predict stock prices and can be easily adapted to other companies and timeframes.</p>

<h1> Requirements </h1>
<ul> <h3> Python version </h3> </ul> 
  <li> Python 3.7 or above </li>
  
  <h2><ul> Installation of Libraries </ul></h2>
     <li>pandas</li>
     <li>numpy</li>
     <li>matplotlib</li>
     <li>seaborn</li>
     <li>pandas_datareader</li>
     <li>yfinance</li>
     <li>datetime</li>
     <li>keras</li>
     <li>scikit-learn</li> 
<h1> Usage </h1>
     <p> After installing the dependencies, open the Python file in a Jupyter Notebook or run it directly from the terminal. The code will download the stock price data for State Bank of India and split it into training and testing datasets. Then it will create an LSTM model, train it on the training data, and use it to predict the stock prices for the testing data.</p>
<h1> Code Structure </h1>
<li>Import the necessary libraries: pandas, numpy, matplotlib, seaborn, pandas_datareader, yfinance, datetime, scikit-learn, and keras.</li>
<li>Define the list of stocks to download the data for and the date range.</li>
<li>Download the data for each stock using yfinance and store it in a dictionary.</li>
<li>Plot the adjusted closing price for each stock using matplotlib.</li>
<li>Scale the data using the MinMaxScaler from scikit-learn.</li>
<li>Split the data into training and testing datasets.</li>
<li>Create the LSTM model using keras.</li>
<li>Train the model on the training data.</li>
<li>Use the model to predict the stock prices for the testing data.</li>
<li>Plot the predicted and actual stock prices using matplotlib.</li>
<li>Calculate the root mean squared error (RMSE) to evaluate the performance of the model.</li>
     
     
