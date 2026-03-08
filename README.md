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

Several preprocessing steps were performed before building forecasting m
