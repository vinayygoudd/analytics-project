# analytics-project
📊 Customer Behavior Analysis — Data Analytics Project
📝 Overview

This project analyzes customer shopping behavior using Python, SQL, and Power BI.
The goal is to uncover insights around customer demographics, spending patterns, category performance, and review behavior.

The workflow demonstrates a complete end-to-end analytics pipeline:

Loading raw data in Python

Running SQL queries directly in Colab

Performing EDA & cleaning

Preparing enriched datasets

Designing a Power BI dashboard

Delivering a clear business-focused report

This project showcases real-world analytics skills across Python, SQL, and BI.

📂 Dataset

Two datasets were used:

File	Description
customer_shopping_behavior.csv	Raw customer transaction data
cleaned_customer_data.csv	Cleaned & transformed dataset

Key attributes include:

Age, gender, yearly salary

Category of purchase

Purchase amount

Review ratings

Shipping type

Subscription status

🛠️ Tools & Technologies
Tool	Purpose
Python (Pandas, NumPy, Matplotlib, Seaborn)	Data loading, cleaning, EDA
SQL (via Google Colab)	Querying, filtering, aggregations, grouping
Jupyter/Google Colab	Interactive workflow
Power BI Desktop	Dashboard creation
GitHub	Version control & hosting
🔍 Steps Performed
1️⃣ Data Loading

Imported raw CSV into Python

Inspected schema, datatypes, nulls, and duplicates

Verified integrity of customer & transaction fields

2️⃣ SQL Queries in Colab

To simulate real database exploration, SQL queries were executed inside the Colab notebook using in-memory SQLite / IPython SQL magic.

SQL tasks performed:

Selecting key columns

Filtering customers by category, gender, subscription

Sorting by purchase amount and ratings

Aggregating revenue & sales by category

Grouping customers by age group

Counting customers by shipping type

Example SQL patterns used:

SELECT category, SUM(purchase_amount) AS revenue
FROM customer_data
GROUP BY category
ORDER BY revenue DESC;

SELECT gender, AVG(review_rating) AS avg_rating
FROM customer_data
GROUP BY gender;


This SQL layer strengthens the analysis by combining database-style exploration with Python EDA.

3️⃣ Exploratory Data Analysis (EDA) in Python

Univariate and bivariate analysis

Revenue patterns across categories

Rating distributions

Detecting skewness and outliers

Creating new features (e.g., Age Groups)

4️⃣ Data Cleaning

Performed in Python:

Removed duplicates

Handled missing values

Fixed inconsistent category labels

Converted data types

Standardized column names

Exported cleaned dataset for Power BI

5️⃣ Dashboard Development in Power BI

Built a clean, interactive dashboard featuring:

KPIs:

Total Customers

Average Purchase Amount

Average Rating

Slicers for:

Gender

Category

Shipping Type

Subscription Status

Charts:

Revenue by Category

Sales by Category

Customer Distribution by Subscription

Revenue by Age Group

Sales by Age Group

📈 Dashboard Preview

(Replace with your actual screenshot in images/)

⭐ Key Insights & Results

Clothing drives the highest revenue and sales

73% of customers are non-subscribers

Young Adults & Middle-aged groups contribute most of the revenue

Average purchase amount ≈ $59.76

Average customer rating = 3.75

Accessories category is the second strongest performer

These insights can support improvements in:

Marketing segmentation

Category-level inventory planning

Pricing & promotions

Subscription program strategies

▶️ How to Run This Project
1. Run Python + SQL Notebook

Open notebook/code.ipynb

Install required libraries:

pip install pandas numpy matplotlib seaborn sqlalchemy


Run all cells to reproduce:

SQL queries

EDA

Cleaning

Exporting the cleaned dataset

2. Open Power BI Dashboard

Download dashboard/Customer_behaviour_Dashboard.pbix

Open in Power BI Desktop

If prompted, relink the cleaned dataset (cleaned_customer_data.csv)

📦 Project Structure
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

📬 Contact

Feel free to connect if you'd like feedback or collaboration on analytics projects.

