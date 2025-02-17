# Stock-Price-Prediction_Simple_Machine-Learning



## Overview
This project explores stock market trends using historical stock data and applies machine learning models to predict stock prices. The dataset is sourced from Yahoo Finance and includes key features such as **Open, High, Low, Close, Adjusted Close, and Volume**.

## Features and Goals
- **Data Preprocessing**: Handling missing values, feature engineering, and transformations.
- **Exploratory Data Analysis (EDA)**: Visualizing market trends and identifying important stock indicators.
- **Feature Engineering**:
  - Log transformation on volume.
  - Calculation of daily returns, moving averages, volatility, and lagged values.
- **Feature Selection**:
  - Recursive Feature Elimination (RFE) with Linear Regression.
  - Feature importance using Random Forest.
- **Modeling**:
  - Linear Regression for stock price prediction.
  - Model evaluation using Mean Squared Error (MSE) and R-squared (R²) score.
- **Visualization**:
  - Feature importance graphs.
  - Actual vs. Predicted price comparison.
  - Residual analysis.

## Dataset
The dataset contains historical stock data with the following columns:
- **Date**
- **Open, High, Low, Close**: Standard stock price data
- **Adj Close**: Adjusted closing price considering splits and dividends
- **Volume**: The number of shares traded

## Installation
To run this project locally, install the required dependencies:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

## Usage
1. Clone this repository:
```bash
git clone https://github.com/yourusername/stock-price-prediction.git
cd stock-price-prediction
```
2. Run the script:
```bash
python main.py
```

## Model Performance
- **Linear Regression MSE**: `11597.728`
- **Linear Regression R²**: `0.9992`
- **Feature Importance** (using Random Forest):
  - Moving Average (30-Day)
  - Moving Average (7-Day)
  - Daily Returns
  - Volatility
  - Log Volume

## Visualizations
- **Stock Price Trends**: Time-series plots of actual vs. predicted values.
- **Feature Importance**: Bar chart of important features based on Random Forest.
- **Residual Analysis**: Distribution of errors to check model performance.

## Future Improvements
- Implement more advanced models (e.g., LSTM, XGBoost).
- Include macroeconomic indicators (e.g., interest rates, inflation).
- Improve feature engineering with additional technical indicators.

## Contributing
If you'd like to contribute, feel free to fork the repository and submit a pull request.

## License
This project is licensed under the MIT License.

