# 🛒 Retail Price Analysis & Prediction (2017–2025)

A comprehensive data analytics and machine learning project that analyzes **118,000+ retail product price records** collected across multiple years, geographies, and product categories. The project uncovers pricing trends, detects anomalies, and builds models to predict and classify retail price levels.

---

## 📌 Project Overview

This project explores how retail product prices vary across:

- Time (month, year, trends)
- Geography (regions)
- Product categories (Food, Fuel, Meat, Dairy, etc.)
- Tax impact (before/after tax)
- Essential vs non-essential items

It applies **exploratory data analysis, anomaly detection, regression, and classification models** to extract insights and build predictive systems relevant to retail pricing.

---

## 📂 Dataset

- **Total Rows:** 118,482  
- **Years:** 2017–2025  
- **Features:** 12 (Category, Tax rate, GEO, Essential flag, Price before/after tax, etc.)  
- **Source:** Kaggle – Retail Prices of Products Dataset  

### Key Columns

- `VALUE` — Price before tax  
- `Value after tax`  
- `Product Category`, `Products`  
- `GEO` — region  
- `Essential` (Yes/No)  
- `Taxable`, `Total tax rate`  
- `Year`, `Month`  

---

## 🛠️ Tech Stack

- Python, Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- LightGBM, XGBoost  
- Isolation Forest  
- GeoPandas (geospatial analysis)  

---

## 🔧 Key Steps Performed

### 1️⃣ Data Cleaning & Feature Engineering

- Created `Date` column using Month + Year  
- Encoded categorical variables  
- Engineered:  
  - `Price_Level` (Low/Medium/High using quantiles)  
  - `Month_num`, `Year_num`  
- Removed nulls and converted dtypes  

---

### 2️⃣ Exploratory Data Analysis

- Boxplots, barplots, heatmaps  
- Category-wise price variation  
- Essential vs non-essential analysis  
- Month/year trends  

**Insight:** Essential goods show lower variation and more stable pricing.

---

### 3️⃣ Time Series Analysis

- Monthly average price trend (2017–2025)  
- Category-based seasonality  

**Insight:** Prices rise steadily post-2020, indicating possible inflation.

---

### 4️⃣ Anomaly Detection

Used **Isolation Forest** to detect unusual price spikes/dips.

**Insight:** Highlights potential supply chain disruptions and abnormal market behavior.

---

### 5️⃣ Regression Modeling (Price Prediction)

Model: **Linear Regression**

| Metric   | Score     |
|----------|-----------|
| RMSE     | **4.001** |
| R² Score | **0.390** |

---

### 6️⃣ Classification Modeling (Price Level Prediction)

Target: **Low / Medium / High price tier**

Models tested:

- Logistic Regression  
- Random Forest  
- Gradient Boosting  
- LightGBM  

#### 🏆 Best Model: Random Forest

| Model                      | Accuracy   |
|----------------------------|------------|
| **RandomForestClassifier** | **83.13%** |
| LightGBM                   | 76.05%     |

---

## 📊 Visualizations

This project includes:

- Boxplots of essential vs non-essential items  
- Category-wise price distribution  
- Monthly & yearly price trends  
- Anomaly detection scatter plots  
- Confusion matrices  

---

## 🚀 Results & Insights

- Meat & Dairy show highest price ranges  
- Strong upward trend in prices after 2020  
- Clear outlier detection patterns  
- Random Forest performs best for price-level classification  

---

## 💡 Future Improvements

- Add ARIMA/Prophet for dedicated forecasting  
- Build Streamlit dashboard  
- Add geospatial price heatmaps  
- Hyperparameter tuning for better ML performance  

---

## 🧑‍💻 Author

**Srijith Chetla**  
Python • Machine Learning • Data Science

---
