# Task 4: Time Series Analysis & Decomposition

## 📌 Project Objective
The goal of this task was to move beyond static data and analyze how revenue changes over time. By using statistical decomposition, I isolated the underlying growth trends and recurring seasonal patterns within the Online Retail dataset.

---

## 📊 1. Daily Revenue & 7-Day Smoothing
To handle the high volatility of daily sales, I applied a **7-Day Moving Average**. This "smooths" out the daily noise to reveal the true direction of the business.

![Daily Revenue Trend](images/Daily%20revenue%20chart.png)

* **Insight:** The red line (Moving Average) shows that while daily sales jump around, the business experienced a significant and sustained "climb" starting in September 2011.

---

## 🔍 2. Seasonal Decomposition
Using the `statsmodels` library, I decomposed the revenue into four distinct components:

![Time Series Decomposition](images/Decompose%20chart.png)

### **Key Component Insights:**
* **Trend:** Confirms a strong upward trajectory toward the end of the year, proving the business is expanding.
* **Seasonal:** Reveals a predictable "heartbeat." The model shows a consistent cycle where seasonal factors provide a **gain of ~10k units** and a **dip of ~20k units** depending on the time of the month/quarter.
* **Resid (Residuals):** Most data points sit near the zero line, which means our Trend and Seasonality models explain almost all of the revenue behavior. The outliers represent "one-off" events like massive bulk orders.

---

## 🗓️ 3. Weekly Revenue Habits
I analyzed the total revenue based on the day of the week to identify peak shopping periods.

![Total Revenue by Day](images/total%20revenue%20by%20day.png)

* **Peak Day:** **Thursday** is the clear winner, driving nearly **2 Million** in total revenue.
* **The Saturday Gap:** There is zero recorded revenue for Saturdays. This suggests either a data recording issue or that the business does not process orders on that day—representing a massive growth opportunity.

---

## 🛠️ Technical Implementation
* **Library:** `statsmodels.tsa.seasonal` (seasonal_decompose)
* **Smoothing:** `rolling(window=7).mean()`
* **Visualization:** Matplotlib / Seaborn
