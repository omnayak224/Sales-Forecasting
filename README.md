# E-Commerce Sales Forecasting Engine

This repository contains an end-to-end Machine Learning pipeline designed to forecast daily revenue for an e-commerce platform. The project demonstrates the full data science lifecycle, from cleaning raw transactional logs to deploying advanced statistical and deep learning predictive models.

## 🚀 Project Overview
Accurate sales forecasting is critical for inventory management and strategic business planning. This project compares three distinct modeling approaches to determine the optimal engine for predicting daily revenue:
1. **Meta Prophet**: A business-focused, curve-fitting model optimized for holiday and promotional spikes.
2. **SARIMAX**: A classical statistical approach capturing seasonality and trend dependencies.
3. **LSTM (Long Short-Term Memory)**: A deep learning neural network designed to capture complex, non-linear sequences in data

## 🛠 Tech Stack
* **Language**: Python 3.x
* **Data Processing**: `Pandas`, `NumPy`
* **Visualization**: `Matplotlib`
* **Modeling**: `Statsmodels` (SARIMAX), `Prophet` (Meta), `TensorFlow/Keras` (LSTM)

## 📈 Methodology
1. **Data Cleaning**: Handled negative transaction quantities (cancellations) and synthesized daily revenue.
2. **Time-Series Aggregation**: Resampled raw receipts into a continuous daily timeline, filling missing dates to ensure index consistency.
3. **Decomposition**: Extracted Trend, Seasonality, and Residual components to understand underlying performance rhythms.
4. **Modeling**:
    * **Prophet**: Incorporated holiday/promotional windows to anticipate year-end spikes.
    * **SARIMAX**: Configured for 7-day weekly cycles.
    * **LSTM**: Implemented a sliding window (window size=14) to capture complex, non-linear patterns.

## 💡 How to run
1. Clone this repository.
2. Install dependencies: `pip install pandas matplotlib statsmodels prophet tensorflow scikit-learn`
3. Run the Jupyter Notebook `Pro _file.ipynb`.

---
*Created by Om Nayak
