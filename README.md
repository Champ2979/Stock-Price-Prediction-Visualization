# Stock-Price-Prediction using (LSTM).
Stock price prediction of State Bank of India and visualization of SBI and Reliance Industries stock
<h1> Overview </h1>
<p> This code is a Machine Learning (ML) program that predicts the stock prices of an Indian company name State Bank of India (SBIN) and visualization of SBI and Reliance Industries Limited (RELIANCE). The program uses historical data from Yahoo Finance to train a Long Short-Term Memory (LSTM) model to predict future stock prices. The program begins by importing the required libraries, including Pandas, Numpy, Matplotlib, Seaborn, and the Yahoo Finance API. Next, it downloads one year of historical data for SBIN and RELIANCE and plots the Adjusted Close price of the stocks. The program then selects the closing price of SBIN for further analysis, scales the data, and creates a training data set using a sliding window technique. The LSTM model is constructed, compiled, and trained using the training data set. The program then creates a testing data set, makes predictions using the trained model, and calculates the Root Mean Squared Error (RMSE) between the predicted values and actual values. Overall, the program provides an example of using an LSTM model to predict stock prices and can be easily adapted to other companies and timeframes.</p>

<h1> Requirements </h1>
<ul> <h3> Python version </h3> </ul> 
  <li> Python 3.7 or above </li>
  
  <h2><ul> Installation of Libraries </ul></h2>
     <li>pandas</li>
     <li>numpy,</li>
     <li>matplotlib, </li>
     <li>seaborn, </li>
     <li>pandas_datareader,</li>
     <li>yfinance, API</li>
     <li>datetime</li>
     <li>keras,</li>
     <li>scikit-learn,</li> 
     
 <h1>Versions (need to install)</h1>
     <h3>pandas</h3>
       <li>Version: 1.5.2</li>
     <h3>numpy</h3>
       <li>Version: 1.24.1</li>
     <h3>matplotlib</h3>
        <li>Version: 1.5.2</li>
     <h3>seaborn</h3>
        <li>Version: 0.12.2</li>
     <h3>pandas_datareader</h3>
        <li> Version: 0.10.0</li>
     <h3>yfinance</h3>
        <li>Version: 0.2.6</li>
     <h3>keras</h3>
        <li>Version: 2.11.0</li>
     <h3>scikit-learn</h3>
        <li>Version: 1.2.0</li>
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
<h1> Concept of moving average </h1>
<p> My approach for predicting the stock prices for State Bank of India is completly based on the project of <strong>moving average</strong>. Moving average is a widely used technical analysis tool that helps to smooth out the price action of a stock or any other financial asset over a specified period of time. In this code, the moving average concept is not explicitly used. However, it is indirectly used when the window size of 60 is specified to create the input sequences for the LSTM model. This window size determines the number of previous time steps (or days) to consider when predicting the next time step. By using a larger window size, the model can capture the long-term trends and patterns in the data, which is similar to what a moving average does.</p>

<h2> Note: </h2> <h4><strong> To predict stock prices, we will only be using the "close" column as input, as stock prices tend to change frequently over time. While other parameters can also be considered, we need to be cautious not to overfit the model by including too many features that may not have a significant impact on the stock prices.</strong></h4>

<h1>Results</h1>
<p>The LSTM model was able to predict the stock prices for State Bank of India with a reasonable accuracy. The RMSE was calculated to be around 3.8, which means that the predicted prices were on average about 3.8 rupees away from the actual prices. The predicted and actual prices were plotted using matplotlib to visualize the performance of the model.</p>

<h1> Conclusion</h1>
<p>This project demonstrates the use of LSTM to predict stock prices. While the model was able to make reasonably accurate predictions for State Bank of India, it may not generalize well to other stocks. Further research is needed to optimize the model and evaluate its performance on other stocks.</p>
<h1> References</h1>
     <li><a href="https://pandas.pydata.org/docs/">Pandas documentation</a></li>
     <li><a href="https://numpy.org/doc/stable/">NumPy documentation</a></li>
     <li><a href="https://matplotlib.org/stable/contents.html">Matplotlib documentation</a></li>
     <li><a href="https://seaborn.pydata.org/">Seaborn documentation</a></li>
     <li><a href="https://pandas-datareader.readthedocs.io/en/latest/">pandas-datareader documentation</a></li>
     <li><a href="https://pypi.org/project/yfinance/">yfinance documentation</a></li>
     <li><a href="https://scikit-learn.org/stable/documentation.html">scikit-learn documentation</a></li>
     <li><a href="https://keras.io/api/">Keras documentation</a></li>
     
