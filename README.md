# Customer Shopping Behavior Analysis

**Author:** charankck    
**Project Type:** Exploratory data analysis, SQL analytics, Power BI dashboard

---

## 🚀 Project Overview
This project analyzes customer shopping behavior using transactional data (3,900 purchases) across product categories to extract insights on spending patterns, customer segments, product preferences, and subscription behavior. The analysis combines Python-based EDA and preprocessing, PostgreSQL business queries, and a Power BI dashboard for visualization. :contentReference[oaicite:2]{index=2}

---

## 📦 Dataset
- **Rows:** 3,900  
- **Columns:** 18  
- **Key features:** Age, Gender, Location, Subscription Status, Item Purchased, Category, Purchase Amount, Season, Size, Color, Discount Applied, Previous Purchases, Purchase Frequency, Review Rating, Shipping Type.  
- **Missing data:** 37 values in `review_rating` (handled by median imputation per category). :contentReference[oaicite:3]{index=3}

---

## 🔬 What I did
1. **Data cleaning & preprocessing** in Python (pandas): type fixes, rename columns to snake_case, missing-value handling, and feature engineering. :contentReference[oaicite:4]{index=4}  
2. **Feature engineering:** e.g. `age_group`, `purchase_frequency_days`. :contentReference[oaicite:5]{index=5}  
3. **Database integration:** loaded cleaned DataFrame into PostgreSQL for SQL analyses. :contentReference[oaicite:6]{index=6}  
4. **Business queries in SQL** to answer operational questions (list below). :contentReference[oaicite:7]{index=7}  
5. **Interactive dashboard** built in Power BI to present insights. :contentReference[oaicite:8]{index=8}

---

## 🧾 Key SQL analyses / Questions answered
- Revenue by gender  
- High-spending users who used discounts  
- Top 5 products by average rating  
- Shipping type comparison (Standard vs Express)  
- Subscribers vs Non-subscribers (avg spend & total revenue)  
- Discount-dependent products (highest % discounted purchases)  
- Customer segmentation: New / Returning / Loyal  
- Top 3 products per category  
- Relationship between repeat buyers (>5 purchases) and subscription uptake  
- Revenue by age group  
(See `/sql/queries.sql` for the full queries.) :contentReference[oaicite:9]{index=9}

---

## 📊 Dashboard
An interactive Power BI dashboard summarizes and visualizes the major insights (filters for category, gender, age_group, subscription status, shipping type). Exported visuals and `.pbix` are included in the repo under `/powerbi/`. :contentReference[oaicite:10]{index=10}

---

## 🛠️ How to run (Local)
### Requirements
- Python 3.8+  
- PostgreSQL (any recent version)  
- Power BI Desktop (for editing the dashboard)  
- Python libraries: `pandas`, `numpy`, `sqlalchemy`, `psycopg2-binary`, `matplotlib`, `seaborn` (optional), `jupyter` (optional)

### Steps
1. Clone the repo:
   ```bash
   git clone https://github.com/charankck/Analysis-of-Customer-behaviour.git
   cd Analysis-of-Customer-behaviour
