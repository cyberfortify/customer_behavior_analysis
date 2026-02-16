# 🛍️ Customer Shopping Behavior Analysis (End-to-End Data Analytics Project)

<img width="853" height="480" alt="dashboard" src="https://github.com/user-attachments/assets/80bb77ec-4937-4e1c-b408-c82610231720" />

## 📌 Overview

This project analyzes **customer shopping behavior** using transactional purchase data to uncover key insights into customer spending patterns, product preferences, subscription trends, and discount-based purchasing behavior.

The analysis follows an **end-to-end data analytics workflow** including Python-based EDA & cleaning, SQL-based business querying, and dashboard reporting using Power BI.

Dataset includes **3,900 purchase transactions** across multiple categories and customer segments. 


## 🎯 Objectives

* Analyze customer purchase behavior and spending trends
* Identify high-revenue customer segments (age group, gender, subscription status)
* Understand product-level performance and top-rated items
* Perform SQL business analysis for decision-making
* Build an interactive Power BI dashboard for stakeholders
* Provide actionable business recommendations


## 📂 Dataset Information

* **Rows:** 3,900
* **Columns:** 18
* **Missing Values:** 37 missing values in *Review Rating* column 

### Key Columns

* **Customer Details:** Age, Gender, Location, Subscription Status
* **Purchase Details:** Item Purchased, Category, Purchase Amount, Season, Size, Color
* **Behavior Data:** Discount Applied, Promo Code Used, Previous Purchases, Purchase Frequency
* **Additional Info:** Review Rating, Shipping Type


## 🛠 Tools & Technologies Used

### 📌 Programming

* Python (Pandas, NumPy)

### 📌 Visualization

* Matplotlib / Seaborn (for EDA charts)
* Power BI (Interactive Dashboard)

### 📌 Database & SQL

* PostgreSQL (Used for business SQL queries and analysis) 
  *(Can also be adapted for MySQL / SQL Server)*

### 📌 Reporting

* PDF Report Documentation
* Gamma (Presentation / PPT)


## 🔄 Project Workflow (Steps)

### 1️⃣ Data Loading (Python)

* Imported dataset using Pandas
* Checked structure using `df.info()` and summary using `df.describe()` 


### 2️⃣ Exploratory Data Analysis (EDA)

Performed EDA to understand:

* Purchase amount distribution
* Category-wise customer interest
* Subscription behavior
* Shipping type performance
* Discount vs non-discount purchase patterns


### 3️⃣ Data Cleaning & Preprocessing

Cleaning steps performed:

* Handled missing values in **Review Rating** using median rating per category 
* Standardized column names to **snake_case**
* Dropped redundant column `promo_code_used`
* Verified discount consistency

### 4️⃣ Feature Engineering

Created new analytical columns:

* `age_group` (binned customer ages)
* `purchase_frequency_days` (derived from frequency details) 


### 5️⃣ Database Integration (PostgreSQL)

* Connected Python with PostgreSQL
* Loaded cleaned dataset into SQL database for business analysis 


## 🧠 SQL Business Analysis (Key Queries)

SQL queries were used to answer real business questions such as:

1. **Revenue by Gender**
2. **High-Spending Discount Users**
3. **Top 5 Products by Review Rating**
4. **Standard vs Express Shipping Spend Comparison**
5. **Subscribers vs Non-Subscribers Revenue & Avg Spend**
6. **Discount-Dependent Products**
7. **Customer Segmentation (New / Returning / Loyal)**
8. **Top 3 Products per Category**
9. **Repeat Buyers vs Subscription Relationship**
10. **Revenue by Age Group** 


## 📊 Power BI Dashboard

An interactive Power BI dashboard was created to visualize key business insights.

### Dashboard Features

* Total customers overview
* Average purchase amount
* Average review rating
* Subscription status distribution
* Revenue by category
* Revenue by age group
* Sales trends by category and age group
* Filters for category, gender, subscription, shipping type 


## 📈 Key Insights & Results

Some important findings from the analysis include:

* **Male customers generated higher revenue** than female customers.
* **Subscribers and non-subscribers showed similar average spend**, but revenue contribution differed.
* **Express shipping users had slightly higher average purchase amounts** compared to standard shipping.
* Top-rated products included items like **Gloves, Sandals, Boots, Hat, and Skirt**.
* Majority customers fall under the **Loyal segment**, indicating strong repeat purchase behavior.
* Certain products were found to be **discount-dependent**, meaning sales heavily rely on discounts. 


## 💡 Business Recommendations

Based on insights, recommended strategies include:

* Promote subscription plans with exclusive benefits
* Launch loyalty reward programs for repeat buyers
* Optimize discount strategy to protect profit margins
* Highlight top-rated products in marketing campaigns
* Focus marketing efforts on high-revenue age groups and express shipping customers 


## ⚙️ How to Run This Project

### ✅ 1. Clone Repository

```bash
git clone https://github.com/cyberfortify/customer-behavior-analysis.git
cd customer-shopping-behavior-analysis
```

### ✅ 2. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn psycopg2
```

### ✅ 3. Run Python Notebook (EDA + Cleaning)

```bash
jupyter notebook notebooks/customer_analysis_eda.ipynb
```

### ✅ 4. Load Data into PostgreSQL

* Create a PostgreSQL database
* Import cleaned dataset into a table
* Run SQL scripts from:

```bash
sql_queries/business_analysis_queries.sql
```

### ✅ 5. Open Power BI Dashboard

Open the `.pbix` file from:

```bash
powerbi_dashboard/customer_behavior_dashboard.pbix
```


## 📌 Deliverables

✔ Cleaned Dataset (CSV)
✔ Python EDA Notebook
✔ SQL Query File
✔ PostgreSQL Database Analysis
✔ Power BI Dashboard
✔ Final Report (PDF)
✔ Presentation (Gamma PPT Export)

## 👨‍💻 Author

**Aditya Vishwakarma**
📌 Data Analyst / Python Developer
