# ✈️ Airline Passenger Forecasting: ARIMA vs. SARIMAX

![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg) 
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg) 
![Statsmodels](https://img.shields.io/badge/Library-Statsmodels-green.svg)

## 📌 Project Overview
This project explores time series forecasting using the classic **Airline Passengers** dataset. The goal is to predict future monthly passenger traffic by analyzing historical trends and seasonal patterns. 

We build and evaluate two different models to compare their performance: **ARIMA** and **SARIMAX**.

---

## 🥊 Model Comparison: ARIMA vs. SARIMAX

When forecasting monthly airline passengers, the data clearly shows an upward trend (increasing passengers over time) and strict seasonality (peaks during summer months). 

| Feature | ARIMA | SARIMAX |
| :--- | :--- | :--- |
| **Full Name** | AutoRegressive Integrated Moving Average | **Seasonal** AutoRegressive Integrated Moving Average |
| **Handles Trend?** | ✅ Yes | ✅ Yes |
| **Handles Seasonality?** | ❌ No | ✅ Yes |
| **Performance** | Captures the general upward trend but completely misses the repeating seasonal peaks and drops. | Successfully maps both the overall growth trend and the complex seasonal cycles. |
| **Verdict** | Used as a baseline model. | **🏆 The Winning Model** |

---

## 📊 Results

The **SARIMAX** model proved to be highly accurate for this dataset, successfully capturing the seasonality that ARIMA missed. 

![SARIMAX Forecast vs Actual](image_4f5222.png)  

**SARIMAX Error Metrics:**
* **Mean Absolute Error (MAE):** `11.97`
* **Mean Squared Error (MSE):** `276.14`
* **Root Mean Squared Error (RMSE):** `16.62`

---

## 🚀 How to Run 

Follow these steps to run the notebook locally on your machine:

**1. Clone the repository:**
```bash
git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
cd your-repo-name
