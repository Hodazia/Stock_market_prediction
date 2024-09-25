## Stock Market Prediction

In this project, given the stocks data, we will be using variants of LSTM models to predict stock prices.

### Dataset

The dataset consists of Infosys stock prices from year 2020 to end of 2023
The dataset is downloaded from yahoo finance website.
The given csv file can be found in file: INFY_DATA.csv

It has the following columns
- `Date`: The day the stock market was open.
- `Open`: Opening price of the stock on that particular day
- `High`: Highest price of the stock on overall day
- `Low` : Lowest price of the stock on overall day
- `Close`: Closing price of the stock on the day
- `Volume` : the total number of shares or stock sold over a given period of time

### Steps followed

1. Data Collection -> .The data should include relevant features such as opening price, closing price, trading volume, and other market indicators like high and low price. 
2. Data Preprocessing -> We will be using different cleaning techniques to ensure that there will be no outliers and missing values.Then the data will be normalized to ensure all features are on a similar scale for effective machine learning model training. 
3. Model Development -> In this phase, we will develop different LSTM  including Vanilla LSTM, Peephole LSTM, and Depth Gated LSTM  models to predict the future closing price trend of the stock along with models like Decision tree and KNN to determine whether to buy or sell the current stock.we have to define the model architecture (number of layers, neurons per layer, activation functions) for each LSTM variant. 
4. Model Training and Evaluation -> We will split the data into training and testing sets.Then all the models will be tested with new sets of data to check accuracy using metrics like Mean Squared Error (MSE) and R-squared and determine which model produces the best accuracy for future prediction.

### Deep Learning Architecture

The architecture used in the given project is LSTM.

![lstmlayer](https://miro.medium.com/max/552/1*L69bb4OirTPvwRvkDLVFng.png)

To know more about the architecture you can refer to:
1. [https://www.geeksforgeeks.org/deep-learning-introduction-to-long-short-term-memory/](https://www.geeksforgeeks.org/deep-learning-introduction-to-long-short-term-memory/) 
2. [https://www.geeksforgeeks.org/long-short-term-memory-lstm-rnn-in-tensorflow/](https://www.geeksforgeeks.org/long-short-term-memory-lstm-rnn-in-tensorflow/)
3. [https://machinelearningmastery.com/gentle-introduction-long-short-term-memory-networks-experts/](https://machinelearningmastery.com/gentle-introduction-long-short-term-memory-networks-experts/)

### How to use the given project
1. Setup your virtual environment 
```bash
python -m venv [ENVIRONMENT_NAME]
```
    e.g. python -m venv myenv

2. Activate the environment
```bash
myenv\Scripts\activate
```
3. Install the required libraries
```bash
python -r requirements.txt
```
4. Run the main.py
```bash
streamlit run main.py
```

### Conclusion
This project’s main objective is to develop a model using machine learning to accurately predict the future stock
prices based on historical data. We will compare the performance of different LSTM variants to determine the most
effective approach for stock price prediction.We will determine which is the best classification model to predict
whether to buy or sell the stock to earn maximum profit.