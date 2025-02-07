# Air Quality Forecasting with LSTM and Machine Learning Models

## Project Overview
This project aims to develop a real-time air quality monitoring and forecasting system using machine learning and deep learning techniques. The models are trained on the "Air Quality Data in India" dataset and include:

- **Random Forest Regressor (RFR)**
- **Support Vector Regressor (SVR)**
- **Long Short-Term Memory (LSTM)**

The project explores different preprocessing methods and evaluates model performance using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R² score.

## Files Overview
### 1. **Air_Quality_LSTM.ipynb**
This notebook implements a deep learning-based approach using Long Short-Term Memory (LSTM) networks for air quality forecasting. Key steps include:

- **Data Preprocessing**
  - Handling missing values
  - Feature selection (PM2.5, NO2, CO, SO2, O3)
  - Scaling and transformation (StandardScaler, log transformation)
  - Sequence creation for time-series forecasting
- **Model Implementation**
  - LSTM network design
  - Training and evaluation with MAE, MSE, and R² score
  - Hyperparameter tuning (window size optimization)
- **Performance Analysis**
  - Comparing results with different preprocessing techniques
  - Observing improvements with log transformation

### 2. **AQI_LSTM.ipynb**
This notebook focuses on machine learning models, specifically Random Forest and Support Vector Regression, for air quality prediction. Key highlights:

- **Exploratory Data Analysis (EDA)**
  - Statistical analysis
  - Correlation analysis
  - Box-plots and scatter plots
- **Model Training & Evaluation**
  - Training RF and SVR models
  - Grid search hyperparameter tuning for SVR
  - Performance comparison of preprocessing methods
- **Results & Observations**
  - Best performance achieved with Random Forest and log-transformed data
  - SVR benefited from hyperparameter tuning

### 3. **Research Paper (Research Paper.docx)**
This document provides an in-depth discussion on the research conducted, covering:

- **Introduction**: Importance of real-time air quality monitoring
- **Literature Review**: Survey of machine learning models used in air quality forecasting
- **Methodology**:
  - Data collection and cleaning
  - Model selection (RF, SVR, LSTM)
  - Hyperparameter tuning
  - Evaluation metrics
- **Findings**:
  - RF model demonstrated the best results with minimal preprocessing
  - SVR improved significantly with hyperparameter tuning
  - LSTM required extensive preprocessing but showed promise with data transformation
- **Challenges & Limitations**:
  - Handling outliers and missing data
  - Computational complexity of deep learning models
- **Deployment Readiness Checklist**
  - Scalability, reliability, and integration requirements

## Summary of Results
| Model  | MAE | MSE | R²  |
|--------|-----|-----|-----|
| RF (No Scaling)  | 18.78 | 1020.37 | 0.84 |
| SVR (No Scaling) | 18.7  | 1104.96 | 0.81 |
| LSTM (No Scaling) | 22.24 | 1121.2 | 0.81 |
| RF (Standard Scaling) | 0.24 | 0.16 | 0.84 |
| SVR (Standard Scaling) | 0.24 | 0.17 | 0.81 |
| LSTM (Standard Scaling) | 0.34 | 0.27 | 0.72 |
| RF (Log Transform) | 0.15 | 0.05 | 0.82 |
| SVR (Log Transform) | 0.16 | 0.05 | 0.79 |
| LSTM (Log Transform) | 0.18 | 0.06 | 0.77 |

## Future Work
- Further optimization of LSTM hyperparameters
- Exploring additional feature engineering techniques
- Implementing real-time data streaming for deployment

This markdown file serves as documentation for the notebooks and research paper, summarizing key insights and results from the project.
