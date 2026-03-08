# ESG Stock Price Forecasting
Time-series forecasting of stock returns using ARIMA, VAR, and LSTM models to evaluate the impact of ESG scores.

## Dataset Source

The dataset used in this project was obtained from Kaggle:

Industrial Sector ESG Ratings and Stock Market Data
https://www.kaggle.com/datasets/jenniferaduffy/industrial-sector-esg-ratings-and-stock-market-data

## Overview

This project explores whether Environmental, Social, and Governance (ESG) factors help improve the prediction of stock returns. The analysis compares traditional time-series models with deep learning approaches to evaluate forecasting performance across companies with different ESG scores.

The main objective is to understand whether ESG information adds meaningful predictive value when modeling daily stock returns.

## Dataset

The dataset contains daily stock price data from 2017 to 2025 along with ESG scores for publicly listed companies. Since ESG values in this dataset remain constant over time, they are used primarily for comparison across firms rather than as dynamic predictors.

To keep the analysis manageable, three companies representing low, medium, and high ESG ratings were selected. This allows us to examine whether model behavior differs across ESG categories.

Source: Kaggle – Industrial Sector ESG Ratings and Stock Market Data

## Data Preparation

Several preprocessing steps were performed before building forecasting models:

Calculation of daily log returns

Creation of lag features for time-series modeling

Rolling volatility measures (7-day and 30-day windows)

Handling missing dates by aligning data to business days

Feature normalization for neural network training

These steps helped transform the raw financial data into a format suitable for both statistical and machine learning models.

Methodology

Multiple forecasting approaches were implemented and compared:

ARIMA (Autoregressive Integrated Moving Average)
Used as a baseline time-series model to capture patterns in stock returns.

ARIMAX
An extension of ARIMA that attempts to include ESG scores as an external variable.

VAR (Vector Autoregression)
Used to analyze interactions between stock returns and volatility.

LSTM (Long Short-Term Memory Network)
A deep learning model designed to capture nonlinear patterns in sequential data.

Model Evaluation

Model performance was evaluated using several metrics:

Mean Absolute Error (MAE)

Root Mean Squared Error (RMSE)

Mean Absolute Percentage Error (MAPE)

Directional accuracy of predicted returns

The Diebold–Mariano test was also used to statistically compare forecasting accuracy between models.

Results

The results indicate that ESG scores in this dataset do not significantly improve short-term forecasting performance. Since ESG values remain constant over time, they do not provide new information for models that rely on dynamic signals.

Across the companies studied, ARIMA models performed similarly to LSTM models, suggesting that more complex deep learning approaches do not necessarily outperform traditional statistical models when the signal-to-noise ratio in the data is low.

The VAR analysis showed expected financial behavior, particularly the persistence of volatility shocks relative to return shocks.

Conclusion

This project demonstrates that static ESG indicators are not sufficient for improving short-term stock return forecasts. While ESG factors may influence long-term financial performance, meaningful forecasting improvements likely require ESG data that changes over time.

The analysis highlights the importance of both data characteristics and model selection when applying machine learning techniques to financial time-series problems.

Tools and Libraries

Python was used for the analysis with common data science libraries such as:

- pandas

- numpy

- statsmodels

- scikit-learn

- tensorflow / keras

- matplotlib

Author

Anshika Kothari
