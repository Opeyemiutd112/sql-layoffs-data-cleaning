# SQL Data Cleaning Project – Global Layoffs Dataset 🗂️

## 👋 Introduction
This project demonstrates my ability to perform **data cleaning in SQL** using a real-world dataset of global layoffs.  

The goal was to **transform raw, messy data into a clean and analysis-ready format** by applying systematic SQL data cleaning steps.

---

## 🎯 Project Objectives
The main objectives of this project were to:
1. Remove **duplicate records** and maintain data integrity.  
2. **Standardize text fields** (industries, countries, company names) for consistency.  
3. Handle **null and missing values** strategically.  
4. Correct **date formats** for time-based analysis.  
5. Drop **unnecessary columns and rows** that cannot add value to analysis.  
6. Prepare a **clean staging table** for exploratory data analysis (EDA) and visualization.  

---

## 📌 Data Cleaning Steps
The following steps were carried out in SQL:

1. **Create a staging table** – to preserve raw data and work on a copy.  
2. **Remove duplicates** – using `ROW_NUMBER()` with `PARTITION BY` logic.  
3. **Standardize values** – 
   - Converted blank industries to `NULL` and filled them with consistent values.  
   - Unified inconsistent categories (e.g., `Crypto Currency`, `CryptoCurrency` → `Crypto`).  
   - Cleaned country names (`United States.` → `United States`).  
4. **Fix data types** – Converted date strings to proper SQL `DATE` format.  
5. **Handle null values** – Left nulls for numerical columns (laid-off counts, funds raised) where data was missing.  
6. **Remove useless rows/columns** – Dropped records where both `total_laid_off` and `percentage_laid_off` were `NULL`.  

---

## 🚀 What Makes This Project Stand Out
- ✅ **SQL-first Approach** – Full data cleaning done using SQL without external tools.  
- ✅ **Reproducible Process** – Structured, step-by-step queries that can be reused on similar datasets.  
- ✅ **Business-Oriented Cleaning** – Ensures the dataset is ready for **trend analysis, industry impact studies, and executive reporting**.  

---

## 🛠️ Tools & Technologies
- **SQL (MySQL / PostgreSQL compatible)** – Data cleaning & transformation.  
- **Kaggle Dataset** – Global Layoffs 2022.  
- **GitHub** – Version control and project documentation.

  ## 📈 Recommendations for Stakeholders
Based on the cleaned dataset, stakeholders (e.g., HR teams, executives, policymakers) can:  

### 1. Business Strategy
- 📉 **Track Layoff Trends** – Identify which industries are most impacted to adjust hiring and investment strategies.  
- 🌍 **Regional Analysis** – Compare layoffs across countries to guide global workforce planning.  
- 🏢 **Company Benchmarking** – Evaluate company layoffs relative to funds raised and growth stage.  

### 2. Workforce & Policy Insights
- 👥 **Employee Support** – Prioritize industries with high layoffs for retraining and outplacement programs.  
- 📊 **Crisis Planning** – Use clean data for forecasting and scenario planning during economic downturns.  
- 🧭 **Policy Decisions** – Governments and labor organizations can focus interventions on highly impacted sectors.  


---
