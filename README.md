# 📊 Customer Behavior Analysis — Data Analytics Project

## 📝 Overview
This project analyzes customer shopping behavior using **Python**, **SQL**, and **Power BI**.  
The goal is to uncover insights related to customer demographics, spending patterns, product category performance, and review behavior.

This project demonstrates a full **end-to-end analytics workflow**:

- Loading raw data in Python  
- Running SQL queries directly inside Colab  
- Performing Exploratory Data Analysis (EDA)  
- Cleaning and transforming data  
- Developing an interactive Power BI dashboard  
- Communicating insights with a business-focused report  

It showcases real-world analytics skills across **Python, SQL, and Business Intelligence**.

---

## 📂 Dataset

Two datasets were used:

| File | Description |
|------|-------------|
| `customer_shopping_behavior.csv` | Raw customer transaction data |
| `cleaned_customer_data.csv` | Cleaned & transformed dataset |

**Key features include:**

- Age, Gender  
- Category of Purchase  
- Purchase Amount  
- Review Ratings  
- Shipping Type  
- Subscription Status  
- Yearly Salary  

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Python (Pandas, NumPy, Matplotlib, Seaborn)** | Data loading, cleaning, analysis |
| **SQL (via Google Colab)** | Querying, filtering, grouping, aggregations |
| **Jupyter / Google Colab** | Notebook environment |
| **Power BI Desktop** | Dashboard creation |
| **GitHub** | Version control & hosting |

---

## 🔍 Steps Performed

### **1️⃣ Data Loading**
- Imported the raw CSV into Python  
- Inspected schema, datatypes, null values, and duplicates  
- Verified integrity of customer & transaction fields  

---

### **2️⃣ SQL Queries in Colab**
SQL queries were executed inside the Colab notebook using in-memory SQLite / IPython SQL magic.

**SQL tasks included:**
- Selecting specific fields  
- Filtering based on category, gender, subscription status  
- Sorting by purchase amount and ratings  
- Aggregating revenue & sales by category  
- Grouping customers by age group  
- Counting customers by shipping type  

**Example SQL queries:**

sql
SELECT category, SUM(purchase_amount) AS revenue
FROM customer_data
GROUP BY category
ORDER BY revenue DESC;

SELECT gender, AVG(review_rating) AS avg_rating
FROM customer_data
GROUP BY gender;
SQL provided a structured way to validate and explore the dataset before visualization.
3️⃣ Exploratory Data Analysis (EDA) in Python

Univariate & bivariate analysis

Revenue trends by category

Rating distribution & behavior

Outlier detection

Feature engineering (e.g., Age Group classification)

4️⃣ Data Cleaning

Performed in Python:

Removed duplicates

Handled missing values

Standardized column names

Corrected inconsistent category labels

Converted columns to proper datatypes

Exported cleaned dataset for dashboarding

5️⃣ Dashboard Development in Power BI

The dashboard includes:

KPIs

Total Customers

Average Purchase Amount

Average Rating

Filters (Slicers)

Gender

Category

Shipping Type

Subscription Status

Visuals

Revenue by Category

Sales by Category

% of Customers by Subscription Status

Revenue by Age Group

Sales by Age Group
⭐ Key Insights & Results

Clothing is the highest-performing category in both revenue and sales

73% of customers are non-subscribers

Young Adults and Middle-aged groups contribute the largest share of revenue

Average purchase amount is $59.76

Average customer rating is 3.75

Accessories rank second-highest in revenue

These insights support:

Better marketing segmentation

Inventory planning

Pricing and discount strategy

Subscription program improvements

▶️ How to Run This Project
1. Run Python + SQL Notebook

Open the notebook:
notebook/code.ipynb

Install required Python libraries:

pip install pandas numpy matplotlib seaborn sqlalchemy


Run all cells to reproduce:

SQL queries

EDA

Cleaning

Exporting cleaned dataset

2. Open the Power BI Dashboard

Download:
dashboard/Customer_behaviour_Dashboard.pbix

Open in Power BI Desktop

If prompted, reconnect the cleaned dataset (cleaned_customer_data.csv)

project/
 ├── data/
 │     ├── raw/
 │     │     └── customer_shopping_behavior.csv
 │     └── cleaned/
 │           └── cleaned_customer_data.csv
 ├── notebook/
 │     └── code.ipynb
 ├── dashboard/
 │     └── Customer_behaviour_Dashboard.pbix
 ├── images/
 │     └── dashboard.png (optional)
 └── README.md
 Feel free to reach out if you'd like feedback or want to collaborate on analytics projects.


