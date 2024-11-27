# Predicting Bitcoin Price Movement Using Time-Series Models

This repository contains a Python-based project aimed at predicting the future movement direction of Bitcoin (BTC) prices using freely available data. The project compares three different machine learning models—LSTM, RNN, and XGBoost—on datasets spanning three time intervals: 1-minute, 1-hour, and 1-day. 

The dataset includes BTC price features such as Open, Close, High, Low, and Volume, and was extracted from the Binance exchange using the [ccxt](https://github.com/ccxt/ccxt) Python package.

---

## Project Overview

### **Objective**
To evaluate and compare the performance of LSTM, RNN, and XGBoost models in predicting BTC price movement direction, based on historical price data.

### **Features**
- **Open**: Opening price of BTC.
- **Close**: Closing price of BTC.
- **High**: Highest price during the time interval.
- **Low**: Lowest price during the time interval.
- **Volume**: Trading volume during the time interval.

---

## Dataset Details

- **Source**: Binance exchange, extracted using `ccxt`.
- **Time Range**: Starting from `2017-08-17 04:00:00`.
- **Time Intervals**: 
  - 1-minute
  - 1-hour
  - 1-day
- **Handling Missing Data**: Missing values were imputed using linear interpolation for consistency.

---

## Models Used

1. **LSTM (Long Short-Term Memory)**  
   A type of recurrent neural network (RNN) specifically designed to model temporal sequences and long-term dependencies.

2. **RNN (Recurrent Neural Network)**  
   A foundational time-series model that captures sequential dependencies.

3. **XGBoost (Extreme Gradient Boosting)**  
   A powerful tree-based algorithm known for its efficiency and performance on tabular data.

---

## Repository Structure
. ├── data/ │ ├── 01-raw_data/ # Contains the raw datasets as extracted │ ├── 02-cleaned_data/ # Contains cleaned and preprocessed datasets ├── models/ # Saved models for LSTM, RNN, and XGBoost ├── notebooks/ # Jupyter notebooks for data analysis, preprocessing, and modeling ├── scripts/ # Python scripts for data extraction, cleaning, and modeling ├── write-up/ # Documentation and findings from the project └── README.md



# Project overview and instructions


---

## Installation and Setup

### **Python Version**
This project uses **Python 3.12**. Please ensure it is installed on your system.

### **Dependencies**
To run this project, install the required Python packages using the provided `requirements.txt` file:
```bash
pip install -r requirements.txt
