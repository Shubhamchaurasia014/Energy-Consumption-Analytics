# ⚡ Power Consumption Analysis & Forecasting

## 📌 Overview

This project analyzes household power consumption data to understand usage patterns and predict future energy demand. It includes data cleaning, exploratory data analysis (EDA), and time series forecasting using the ARIMA model.

---

## 📂 Dataset

* Dataset: *Household Power Consumption Dataset*
* Format: `.txt` file (semicolon-separated)
* Features include:

  * Global Active Power
  * Global Reactive Power
  * Voltage
  * Date & Time

---

## ⚙️ Project Workflow

### 1. Data Loading

* Imported dataset using Pandas
* Checked dataset shape and structure

### 2. Data Cleaning

* Replaced missing values (`?`) with null
* Removed null values
* Converted columns to appropriate data types
* Combined **Date + Time → DateTime**
* Set DateTime as index
* Dropped unnecessary columns

---

### 3. Exploratory Data Analysis (EDA)

* **Monthly power consumption trends** using resampling
* **Average daily consumption** calculated
* **Peak usage hours** identified
* **Correlation heatmap** to understand relationships between features

---

### 4. Time Series Forecasting

* Resampled data to daily averages
* Split data into training (80%) and testing (20%)
* Applied **ARIMA model** for forecasting
* Predicted power consumption for next 7 days

---

### 5. Model Evaluation

* Evaluated performance using:

  * MAE (Mean Absolute Error) ~ 0.398
  * RMSE (Root Mean Squared Error) ~ 0.498

---

## 📊 Key Insights

* Power consumption shows consistent **daily and monthly patterns**
* Certain hours exhibit **peak energy usage**
* Strong correlations exist between electrical variables
* ARIMA model captures short-term trends reasonably well

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Statsmodels (ARIMA)

---

## 🚀 Conclusion

The project demonstrates how time series analysis can be used to understand and forecast power consumption. These insights can help in optimizing energy usage and improving decision-making.

---
