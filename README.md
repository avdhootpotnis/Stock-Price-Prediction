# Stock Price Prediction Using Support Vector Regression (SVR)

This project demonstrates how to predict stock prices using Support Vector Regression (SVR) with three kernel types: Radial Basis Function (RBF), Linear, and Polynomial. This code is designed for educational purposes, illustrating a basic approach to machine learning in stock price prediction.

## Project Overview

The aim of this code is to load historical stock price data, preprocess it, and use SVR to predict future prices. We visualize the results of three SVR models and their fitting to the data. **Please note**: This code is a demonstration and should **not** be used for actual trading purposes.

## How It Works

### 1. Import Libraries
The code uses:
- `pandas` to load and preprocess the dataset,
- `numpy` for reshaping data arrays,
- `sklearn.svm.SVR` for the SVR models,
- `matplotlib` to visualize the data and model predictions.

### 2. Data Loading and Preprocessing
The `load_and_preprocess_data()` function:
- Loads the data from the CSV file.
- Extracts the year from each date for model simplicity.
- Converts the "Close/Last" column to numeric after removing currency symbols.

The function returns lists of years and closing prices for further processing.

### 3. Model Training
In `train_svr_models()`:
- Three SVR models are defined, each with a different kernel:
  - **RBF kernel**: Effective for non-linear data patterns.
  - **Linear kernel**: Useful for linear relationships.
  - **Polynomial kernel**: Captures more complex relationships depending on the degree.

Each model is trained using the reshaped years and prices, allowing them to learn the historical price trend.

### 4. Visualization of Results
In `visualize_results()`, we plot the actual data points and the predictions from each of the SVR models. This visualization helps compare how each model type fits the historical data.

### 5. Predicting Stock Prices
The `predict_price()` function allows you to predict prices for a given year using each SVR model. It returns the predicted values from the RBF, Linear, and Polynomial models.

### Disclaimer
*This code is for demonstration purposes only and is not intended for use in trading or financial decision-making. Stock market data is highly volatile and subject to various external factors. The author assumes no responsibility for any potential losses incurred from using this code in any investment-related activities.*

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://pandas.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/2ae2a900d2f041da66e950e4d48052658d850630/icons/pandas/pandas-original.svg" alt="pandas" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://scikit-learn.org/" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg" alt="scikit_learn" width="40" height="40"/> </a> </p>

