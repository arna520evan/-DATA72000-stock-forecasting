# DATA72000 Extended Research Project
## A Machine Learning Approach to Forecasting Stock Prices

This repository contains the code and supporting materials for my MSc Data Science Extended Research Project at The University of Manchester.

## Project Overview

This study compares statistical, machine-learning and deep-learning approaches for next-trading-day stock forecasting across Apple (AAPL), Microsoft (MSFT) and NVIDIA (NVDA).

The main experiments include:

- ARIMA, Random Forest and LSTM model comparison
- GRU and BiLSTM recurrent-model refinements
- direct-price versus return-target LSTM forecasting
- rolling-origin ensemble forecasting
- ARIMA-GARCH residual-volatility analysis

## Data Access

The market data used in this project are publicly available through Yahoo Finance and are retrieved programmatically using the `yfinance` Python package.

The principal analysis uses AAPL, MSFT and NVDA data from 2010 to June 2026.

Raw market data are not redistributed in this repository. The supplied notebook contains the code required to retrieve and preprocess the data used in the analysis.

## Main File

`stock_forecasting_analysis.ipynb`

This notebook contains the final verified implementation used to generate the reported results.

## Software Requirements

The analysis was conducted in Python using packages including:

- pandas
- numpy
- yfinance
- scikit-learn
- statsmodels
- tensorflow / keras
- arch
- scipy
- matplotlib

Exact package dependencies are provided in `requirements.txt`.

## Reproducibility

The analysis preserves chronological order throughout model development and evaluation. Final-test observations are not used for model selection.

Some neural-network experiments use random seeds 42, 123 and 2026.

## Author

Paifeng Peng  
MSc Data Science – Computer Science Data Informatics  
The University of Manchester
