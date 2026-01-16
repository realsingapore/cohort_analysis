# 📊 Cohort Analysis & Customer Retention Dashboard (E-commerce)

## 📌 Project Overview
This project performs an end-to-end **customer retention and churn analysis** for an e-commerce business using **cohort analysis**, **rolling retention**, and **survival analysis**.  
The insights are operationalized into a **production-ready interactive dashboard** built with Streamlit.

The goal is to understand **how long customers stay active**, **when churn happens**, and **which customer segments drive the most revenue**, enabling data-driven retention strategies.

---

## 🎯 Business Objectives
- Measure customer retention over time using cohort analysis
- Identify early vs late churn patterns
- Quantify customer lifetime and churn probability
- Analyze revenue concentration by tenure and geography
- Provide actionable recommendations to improve customer retention
- Deploy insights in a production-ready dashboard

---

## 🗂 Dataset Description
The dataset contains transactional e-commerce data with the following fields:

| Column | Description |
|------|-------------|
| InvoiceNo | Unique transaction identifier |
| InvoiceDate | Date and time of transaction |
| CustomerID | Unique customer identifier |
| StockCode | Product identifier |
| Description | Product category |
| Quantity | Number of units purchased |
| UnitPrice | Price per unit |
| Country | Customer country |

---

## 🧠 Methodology

### 1️⃣ Data Cleaning & Validation
- Converted dates to datetime format
- Removed transactions with missing `CustomerID`
- Removed cancelled invoices
- Validated quantity and price values

### 2️⃣ Cohort Analysis
- Defined cohorts based on **first purchase month**
- Calculated **cohort index** (months since acquisition)
- Built retention and churn matrices
- Visualized retention using heatmaps

### 3️⃣ Churn Analysis
- Computed churn as the complement of retention
- Analyzed customer tenure distribution
- Identified early-stage churn as the primary loss point

### 4️⃣ Advanced Analytics
- **Rolling Retention** to measure long-term engagement
- **Survival Analysis (Kaplan–Meier)** to model customer lifetime
- Estimated median customer lifetime
- Analyzed revenue vs tenure

### 5️⃣ Production Dashboard
- Built an interactive Streamlit dashboard
- KPIs, cohort heatmaps, churn curves, survival plots
- Country-level revenue analysis
- Ready for deployment and stakeholder use

---

## 🧪 Key Insights
- Customer churn is heavily **front-loaded** after the first purchase
- Retention stabilizes after ~3 months
- Long-tenure customers generate **disproportionate revenue**
- A small number of countries drive most revenue
- Retention improvements yield higher ROI than acquisition

---

## 💡 Business Recommendations
- Improve onboarding and first-purchase experience
- Introduce early retention incentives (2nd-purchase offers)
- Protect high-tenure, high-value customers
- Use country-specific retention strategies
- Track Month-2 retention as a leading KPI

---

## 🧰 Tech Stack
- **Python**
- **Pandas / NumPy**
- **Matplotlib / Seaborn**
- **Lifelines (Survival Analysis)**
- **Streamlit (Dashboard)**
- **Jupyter Notebook**
- **Git & GitHub**

---

## 📁 Project Structure
```text
cohort-retention-project/
│
├── Dataset_ecommerce.csv
├── cohort_analysis.ipynb
├── retention_dashboard.py
└── README.md
