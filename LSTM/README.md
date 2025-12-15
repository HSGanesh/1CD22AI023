# LSTM-Based Time Series Forecasting

This project demonstrates **time series forecasting using Long Short-Term Memory (LSTM)** networks implemented with **TensorFlow / Keras**.  
The model is trained on a **built-in synthetic time-series dataset**, eliminating the need for external files or local file paths.

---

##  Objective
To design and train an **LSTM neural network** capable of predicting future values of a time series based on historical observations.

---

##  Dataset Description
- A **synthetic time-series dataset** generated using NumPy
- Combines:
  - Sinusoidal trend
  - Random noise
- Fully reproducible and built-in (no external CSV files)

✔ Meets assignment requirement of avoiding file paths

---

## Modifications Made (IMPORTANT)

The original code was modified as follows:

1️ **Removed external CSV file dependency**  
- Eliminated hard-coded file paths

2️ **Used built-in dataset generation**  
- Time series generated programmatically using NumPy

3️ **Preserved all visualizations**
- Original time-series plot
- Training vs testing prediction plots

4️ **Modularized dataset preparation**
- Created reusable function for time-series windowing

5️ **Retained evaluation metrics**
- Root Mean Squared Error (RMSE) used for performance evaluation

---

##  Model Architecture
- LSTM layer with 10 memory units
- Fully connected Dense output layer
- Loss function: Mean Squared Error
- Optimizer: Adam

---

##  Training Details
- Train-test split: 75% / 25%
- Time window (look-back): 10 steps
- Epochs: 50
- Batch size: 1

---

##  Visualizations Included
1. **Original Time Series Plot**
2. **Training Prediction vs Actual Values**
3. **Testing Prediction vs Actual Values**
4. **Learning behavior visualization**

These plots help analyze the forecasting accuracy of the LSTM model.

---

##  Performance Metrics
- **Train RMSE**
- **Test RMSE**

Lower RMSE values indicate better prediction accuracy.

---

##  Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- TensorFlow / Keras
- Scikit-learn
