# gold-price-prediction-sentiment

# Gold Price Prediction with Market Sentiment Analysis

## Project Overview

This project aims to predict **gold prices** by analyzing their relationship with the **U.S. Dollar Index (DXY)** and incorporating **market sentiment analysis** from global news headlines. The project leverages various time series forecasting models, including:

1. **ARIMA (AutoRegressive Integrated Moving Average)**
2. **SARIMAX (Seasonal ARIMA with Exogenous Factors)**
3. **Prophet (Facebook's Forecasting Tool)**
4. **Hybrid VAR + LSTM (Vector AutoRegression and Long Short-Term Memory)**

---

## Objectives

- **Analyze Historical Data**:
  - Perform Exploratory Data Analysis (EDA) on gold prices, DXY, and sentiment data.
  - Identify trends, seasonality, and correlations.

- **Predict Gold Prices**:
  - Develop time series forecasting models.
  - Compare model performance using RMSE.

- **Incorporate Market Sentiment**:
  - Use Natural Language Processing (NLP) to analyze sentiment from news headlines.
  - Examine the impact of market sentiment on gold prices.

---
## Tools and Libraries

- **Python Libraries**:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - `statsmodels`
  - `fbprophet`
  - `tensorflow`
  - `nltk` (for NLP and sentiment analysis)

- **Jupyter Notebook** for interactive data analysis.

---

## Methodology

### 1. **Exploratory Data Analysis (EDA)**

- Visualize trends and seasonality in gold prices and DXY.
- Analyze market sentiment scores derived from news headlines.
- Conduct correlation analysis between gold prices, DXY, and sentiment.

### 2. **Stationarity Validation**

- Perform the Augmented Dickey-Fuller (ADF) test to ensure data is stationary.

### 3. **Prediction Models**

#### ARIMA Model
- **Parameters**: (1, 1, 1)
- **RMSE**: 104.50

#### SARIMAX Model
- **Parameters**: (1, 1, 1) with exogenous factors (DXY, sentiment).
- **RMSE**: 89.96

#### Prophet Model
- Incorporates seasonal components and external regressors.
- **RMSE**: 86.04

#### Hybrid VAR + LSTM Model
- Combines VAR for multivariate relationships and LSTM for sequential data.
- **RMSE**: High (requires refinement).

---

## How to Run the Project

1. **Clone the Repository**:
   ```bash
   git clone [https://github.com/yourusername/gold-price-prediction-sentiment.git](https://github.com/LoveselvanGit/gold-price-prediction-sentiment.git)
   pip install pandas numpy matplotlib seaborn statsmodels fbprophet tensorflow nltk

import nltk
nltk.download('vader_lexicon')

jupyter notebook DSC630_MAHALINGAM_FINAL_PROJECT.ipynb

Results
Model Performance Comparison
Model	RMSE
ARIMA	104.50
SARIMAX	89.96
Prophet	86.04
Hybrid VAR+LSTM	High Error
Best Performing Model: Prophet (RMSE: 86.04)
Strong Performance: SARIMAX (RMSE: 89.96)

Recommendations
For Investors:
Use Prophet model predictions for investment decisions.
Consider market sentiment and DXY trends for optimal timing.
Future Improvements:
Enhance sentiment data quality for better prediction accuracy.
Refine the Hybrid VAR+LSTM model to reduce error rates.

References
Data Sources:

Auronum Gold Prices
MarketWatch DXY Data
Kaggle Sentiment Dataset
Model References:

ARIMA: Machine Learning Plus
SARIMAX: GeeksforGeeks
Prophet: Facebook Prophet
LSTM: Machine Learning Mastery



