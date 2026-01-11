# Customer Shopping Behavior Analysis

## 📌 Project Overview

This project analyzes customer shopping behavior using transactional data from **3,900 purchases** across multiple product categories. The objective is to uncover actionable insights related to **spending patterns, customer segmentation, product preferences, discounts, and subscriptions** to support data-driven business decisions.

The project demonstrates an **end-to-end data analytics workflow** using **Python, SQL (MySQL), and Power BI**.

---

## 📊 Dataset Summary

* **Rows:** 3,900
* **Columns:** 18
* **Key Features:**

  * Customer demographics: `age`, `gender`, `location`, `subscription_status`
  * Purchase details: `item_purchased`, `category`, `purchase_amount`, `season`, `size`, `color`
  * Shopping behavior: `discount_applied`, `promo_code_used`, `previous_purchases`, `purchase_frequency`, `review_rating`, `shipping_type`
* **Missing Values:** 37 missing values in the `review_rating` column

---

## 🐍 Exploratory Data Analysis (Python)

EDA and data preparation were performed using **Python (pandas, numpy)**.

### Key Steps:

* **Data Loading & Inspection**

  * Used `pandas` to load data
  * Reviewed structure with `df.info()` and statistics using `df.describe()`

* **Missing Data Handling**

  * Imputed missing `review_rating` values using the **median rating per product category**

* **Data Cleaning & Standardization**

  * Renamed columns to **snake_case** for consistency

* **Feature Engineering**

  * Created `age_group` by binning customer ages
  * Derived `purchase_frequency_days` from purchase data

* **Redundancy Check**

  * Identified overlap between `discount_applied` and `promo_code_used`
  * Dropped `promo_code_used`

* **Database Integration**

  * Loaded cleaned dataset into **MYSQL** for SQL-based analysis

---

## 🗄️ Data Analysis (SQL – MYSQL)

Business-focused SQL queries were written to answer key questions:

1. Revenue comparison by **gender**
2. High-spending customers who **used discounts**
3. **Top 5 products** by average review rating
4. Average purchase amount by **shipping type**
5. **Subscribers vs Non-Subscribers** revenue comparison
6. Products most dependent on **discounted purchases**
7. Customer segmentation: **New, Returning, Loyal**
8. **Top 3 products per category**
9. Relationship between **repeat buyers and subscriptions**
10. Revenue contribution by **age group**

---

## 📈 Power BI Dashboard

An interactive **Power BI dashboard** was created to visualize:

* Revenue trends
* Customer segmentation
* Subscription impact
* Product and category performance
* Age group and shipping behavior insights

The dashboard enables quick decision-making through dynamic filters and visuals.

---

## 💡 Business Recommendations

* **Boost Subscriptions:** Offer exclusive deals and benefits for subscribers
* **Loyalty Programs:** Reward repeat buyers to convert them into loyal customers
* **Optimize Discount Strategy:** Balance sales growth with profit margins
* **Product Positioning:** Promote top-rated and best-selling products
* **Targeted Marketing:** Focus on high-revenue age groups and express shipping users

---

## 🛠️ Tools & Technologies

* **Python:** pandas, numpy
* **Database:** MySQL
* **BI Tool:** Power BI
* **IDE:** VS Code / Jupyter Notebook

---

## 📁 Repository Structure

```
├── data/
│   └── customer_shopping_data.csv
├── notebooks/
│   └── eda_data_cleaning.ipynb
├── sql/
│   └── business_queries.sql
├── powerbi/
│   └── customer_behavior_dashboard.pbix
├── README.md
```

---

## 🚀 Future Enhancements

* Predictive modeling for customer churn
* Recommendation system for products
* Automated ETL pipeline
* Advanced customer lifetime value (CLV) analysis

---

## 📌 Author

**Abhishek H**
Data Analyst | Python | SQL | Power BI

---

⭐ If you find this project useful, feel free to star the repository!
