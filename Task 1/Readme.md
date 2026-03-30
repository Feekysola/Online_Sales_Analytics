# Task 1: Data Cleaning & Business Insights 🔍

## 🎯 Project Objective
The goal of this phase was to transform a raw, unstructured online retail dataset into a "Single Source of Truth." By applying rigorous data cleaning and engineering, I aimed to answer critical business questions regarding revenue drivers, seasonality, and customer concentration.

---

## 🛠️ The Data Engineering Process

Raw data is rarely ready for analysis. To ensure the integrity of the findings, I implemented the following pipeline:

1. **Handling Missing Values:** Dropped records with missing `CustomerID` to ensure revenue could be accurately attributed to specific clients.
2. **Transactional Cleaning:** Removed cancellations and returns (identified by negative quantities and "C" prefixes) to focus exclusively on successful sales.
3. **Data Refinement:** Successfully refined the dataset from over 540,000 raw rows to **392,733 validated records**.
4. **Feature Engineering:** - Created a `Revenue` column ($Quantity \times UnitPrice$).
   - Extracted `Month` and `Year` features from the `InvoiceDate` to enable time-series analysis.

---

## 📈 Business Questions & Visualizations

To understand the business health, I formulated and answered several key questions:

### 1. Who are our most valuable customers?
By aggregating revenue by `CustomerID`, I identified the top 5 spenders. This reveals a high concentration of revenue within a small group of high-value accounts.
![Top 5 Customers](./top%205%20customers.png)

### 2. What is our monthly revenue trend?
This visualization shows the business's growth trajectory, highlighting a massive surge in **November**, likely driven by holiday sales preparations.
![Monthly Revenue](./Monthly%20Revenue.png)

### 3. Which international markets are strongest?
Excluding the home market (UK), this analysis identifies which countries offer the most significant growth opportunities for international expansion.
![Top Non-UK Countries](./Top%20non%20Uk%20countries.png)

---

## 🧩 Key Takeaways
- **Cleaning is Critical:** Removing returns and nulls significantly changed the mean revenue, proving that raw data would have led to biased business decisions.
- **Seasonality:** The business is heavily dependent on the Q4 holiday window.
- **Concentration Risk:** A significant portion of revenue is tied to the top 5 customers, suggesting a need for a "VIP" loyalty strategy.

---
[⬅️ Back to Main Project Page](../README.md)
