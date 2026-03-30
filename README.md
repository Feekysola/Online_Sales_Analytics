# 🛒 Online Retail Data Analytics Project

This repository documents a multi-phase end-to-end data analysis of a large-scale Online Retail dataset. The project transitions from raw data engineering to advanced statistical discovery and predictive modeling.

---

## 📂 Project Structure & Objectives

### [📍 Phase 1: Data Cleaning & Business Insights](https://github.com/Feekysola/Online_Sales_Analytics/blob/main/Task%201/Readme.md)
**Primary Objective:** To transform a raw dataset of 500k+ records into a validated "Single Source of Truth" and answer core business performance questions.
* **Key Focus:** Data integrity, handling missing values, and identifying top-tier revenue drivers (Customers, Countries, and Seasons).
* **Final Cleaned Dataset:** 392,733 records.

### [📊 Phase 2: Statistical Exploratory Data Analysis (EDA)](https://github.com/Feekysola/Online_Sales_Analytics/blob/main/Task%202/Readme.md)
**Primary Objective:** To perform a deep-dive statistical validation of the data to uncover hidden relationships and behavioral patterns.
* **Key Focus:** Distribution analysis, outlier detection (The "Whale" Effect), and correlation testing between Quantity and Revenue.
* **Core Finding:** Identified a **0.91 Pearson Correlation** between Quantity and Revenue.

### [🤖 Phase 3: Predictive Analysis (Linear Regression)](https://github.com/Feekysola/Online_Sales_Analytics/blob/main/Task%202/Readme.md)
**Primary Objective:** To build a mathematical framework to forecast revenue based on the volume trends identified in Phase 2.
* **Key Focus:** Implementing a **Linear Regression model** to predict revenue.
* **Core Finding:** The model achieved an **$R^2$ score of 0.73**, proving that quantity is a statistically reliable predictor of total income.

### [📈 Phase 4: Time Series Analysis & Decomposition](https://github.com/Feekysola/Online_Sales_Analytics/blob/main/Task%204/ReadMe.md)
**Primary Objective:** To isolate long-term growth trends from recurring seasonal habits and identify peak operational windows.
* **Key Focus:** Statistical decomposition (Trend, Seasonality, Residuals) and Daily Revenue Habit tracking.
* **Core Finding:** Identified a stable **4-month seasonal cycle** with a predictable +10k/-20k unit variance and confirmed **Thursday** as the primary revenue driver.

---

## 🛠️ Technical Stack
* **Language:** Python 3.x
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn, Statsmodels
* **Tooling:** Jupyter Notebooks, VS Code, Git/GitHub

---

## 🏆 Final Project Outcomes
- **Predictive Accuracy:** Established a model that explains 73% of revenue variance.
- **Strategic Growth:** Confirmed a steady upward trend leading into the Q4 holiday period.
- **Operational Timing:** Identified Thursday as the highest revenue-generating day, allowing for optimized marketing and inventory scheduling.

---
[⬅️ Back to Portfolio](https://github.com/Feekysola)
