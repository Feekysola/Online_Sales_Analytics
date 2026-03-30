# Task 2: Statistical EDA & Predictive Modeling (Linear Regression) 📊

## 🎯 Project Objective
In this phase, I moved beyond standard business reporting to perform deep-dive statistical validation and predictive modeling. The goal was to understand data distribution, isolate high-value anomalies, and build a mathematical framework to predict revenue based on purchase volume.

---

## 🔬 Statistical Discovery & Methodology

### 1. Revenue Distribution (The Skew)
Analysis of the transaction data revealed a heavily right-skewed distribution. The gap between the **Mean (£22.63)** and **Median (£12.39)** indicates that average metrics are pulled upward by a small percentage of high-value orders.

### 2. Outlier Detection: The "Whale" Effect 🐋
Using Boxplot analysis, I identified several extreme outliers in the revenue data, with individual transactions exceeding **£170,000**.
* **Insight:** These represent critical B2B "Whale" accounts that drive significant revenue and require specialized retention strategies.

### 3. Correlation: Quantity vs. Revenue
To understand what truly drives the bottom line, I analyzed the relationship between the number of items sold and the total revenue generated.
* **The "Secret Sauce":** There is a **0.91 Pearson Correlation** between Quantity and Revenue.

---

## 🤖 Predictive Modeling: Linear Regression
Building on the high correlation identified in the EDA, I implemented a **Linear Regression model** using `Scikit-Learn` to predict Revenue based on Quantity.

![Quantity vs Revenue Regression](images/Regression%20chart.png)

### **Model Performance & Findings:**
* **$R^2$ Score (Coefficient of Determination): 0.73**
* **Insight:** Our model explains **73% of the variance** in revenue based on quantity alone. The "Prediction Line" (shown in red) provides a reliable baseline for forecasting sales. 
* **The Outlier Impact:** While the model is highly accurate for the majority of data points, the extreme "Whale" outliers (visible in the top right) suggest that a separate model may be needed for B2B vs. B2C segments.

---

## 💡 Strategic Recommendations
- **Volume Incentives:** Since Quantity is the primary driver of Revenue ($r=0.91$), the business should focus on bundle deals to increase units per transaction.
- **Predictive Forecasting:** The $R^2$ of 0.73 allows the finance team to use this regression model to forecast monthly revenue with a high degree of statistical confidence.
- **B2B Strategy:** The regression gap for high-volume orders confirms that B2B clients behave differently and should be handled with custom pricing tiers rather than standard retail pricing.

---

## 🚀 Future Work
With the predictive relationship between volume and price established, the project moves into **Task 4: Time Series Analysis**, where we will analyze how these trends evolve over time and identify seasonal "heartbeats."

---
[⬅️ Back to Main Project Page](../README.md)
