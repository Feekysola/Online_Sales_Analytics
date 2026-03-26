# 🛒 Online Retail Data Analytics Project

This repository document a two-phase end-to-end data analysis of a large-scale Online Retail dataset. The project transitions from raw data engineering to advanced statistical discovery.

---

## 📂 Project Structure & Objectives

### [📍 Phase 1: Data Cleaning & Business Insights](Task 1)]
**Primary Objective:** To transform a raw dataset of 500k+ records into a validated "Single Source of Truth" and answer core business performance questions.
* **Key Focus:** Data integrity, handling missing values, and identifying top-tier revenue drivers (Customers, Countries, and Seasons).
* **Final Cleaned Dataset:** 392,733 records.

### [📊 Phase 2: Statistical Exploratory Data Analysis (EDA)](./Task_2_Folder_Name/README.md)
**Primary Objective:** To perform a deep-dive statistical validation of the data to uncover hidden relationships and behavioral patterns.
* **Key Focus:** Distribution analysis, outlier detection (The "Whale" Effect), and correlation testing between Quantity, Price, and Revenue.
* **Core Finding:** Identified a **0.91 Pearson Correlation** between Quantity and Revenue.

---

## 🛠️ Technical Stack
* **Language:** Python 3.x
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
* **Tooling:** Jupyter Notebooks

---

## 🚀 Next Steps
This project is currently moving into **Level 2**, where I will be building **Linear Regression Models** to predict future revenue based on the volume trends identified in Phase 2.
