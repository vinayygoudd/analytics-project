# 🛍️ Customer Behavior Analysis — Data Analytics Project  
### **By: Dudala Vinay Kumar Goud**

---

## 📌 **Project Overview**
This project analyzes customer shopping behavior using **Python, SQL, and Power BI** to uncover insights about:

- Customer demographics  
- Spending patterns  
- Product category performance  
- Review and rating behavior  
- Subscription and shipping preferences  

It demonstrates a full **end-to-end data analytics workflow**, including:

1. Loading & inspecting raw data  
2. Running SQL queries directly inside Google Colab  
3. Performing Exploratory Data Analysis (EDA)  
4. Cleaning & transforming the dataset  
5. Building an interactive **Power BI Dashboard**  
6. Communicating insights through visual analytics  

This project reflects real-world analytics tasks performed by Data Analysts and Business Intelligence professionals.

---

## 📂 **Dataset Description**

Two datasets were used:

| File | Description |
|------|-------------|
| **customer_shopping_behavior.csv** | Raw customer transaction data |
| **cleaned_customer_data.csv** | Cleaned & transformed final dataset |

### 📌 Key Dataset Features
- **Demographics:** Age, Gender  
- **Behavior:** Category of Purchase, Purchase Amount, Review Rating  
- **Logistics:** Shipping Type  
- **Customer Value:** Subscription Status, Yearly Salary  

---

## 🛠️ **Tools & Technologies**

| Tool | Purpose |
|------|---------|
| **Python (Pandas, NumPy, Matplotlib, Seaborn)** | Data loading, cleaning, and EDA |
| **SQL (via Google Colab + SQLite)** | Querying, filtering, aggregations |
| **Google Colab / Jupyter Notebook** | Notebook-based workflow |
| **Power BI Desktop** | Dashboard and report creation |
| **GitHub** | Version control and project hosting |

---

## 🔍 **Steps Performed**

### **1️⃣ Data Loading & Inspection**
- Loaded raw CSV into Python  
- Verified schema, datatypes, null values, and duplicates  
- Checked data consistency for customer & transaction fields  

---

### **2️⃣ SQL Queries in Google Colab**
Used IPython SQL magic / SQLite to run structured SQL queries such as:

```sql
SELECT category, SUM(purchase_amount) AS revenue 
FROM customer_data 
GROUP BY category 
ORDER BY revenue DESC;
```

```sql
SELECT gender, AVG(review_rating) AS avg_rating 
FROM customer_data 
GROUP BY gender;
```

SQL helped validate patterns before deeper EDA.

---

### **3️⃣ Exploratory Data Analysis (Python)**
Performed univariate & bivariate analysis to understand:

- Revenue distribution  
- Category performance  
- Rating distribution  
- Age-group behavior  
- Outliers & skewness  
- Correlations  

Created features such as **Age Groups** for improved segmentation.

---

### **4️⃣ Data Cleaning & Transformation**
- Removed duplicates  
- Handled missing values  
- Standardized column names  
- Corrected inconsistent categories  
- Converted datatypes (age → int, rating → float, etc.)  
- Exported the cleaned dataset for visualization  

---

### **5️⃣ Power BI Dashboard Development**
Developed an interactive dashboard showing:

### **KPIs**
- Total Customers  
- Average Purchase Amount  
- Average Rating  
- Subscriber % vs Non-Subscriber %  

### **Filters (Slicers)**
- Gender  
- Category  
- Subscription Status  
- Shipping Type  

### **Visuals**
- Revenue by Category  
- Sales Count by Category  
- Customer Distribution by Subscription  
- Revenue by Age Group  
- Rating Distribution  

---

## ⭐ **Key Insights & Results**

### 🔹 Category Performance
- **Clothing** is the highest-performing category (revenue + volume).  
- **Accessories** rank second in total revenue.

### 🔹 Subscription Behavior
- **73% of customers are non-subscribers** → Large opportunity for subscription program growth.

### 🔹 Customer Segments
- **Young Adults** & **Middle-Aged** groups contribute most to total revenue.

### 🔹 Spending & Ratings
- **Average Purchase Amount:** $59.76  
- **Average Rating:** 3.75 (moderate satisfaction)

### 🔹 Business Impact
Insights help drive:
- Targeted marketing  
- Inventory planning  
- Improved rating strategies  
- Better subscription design  

---

## ▶️ **How to Run This Project**

### **1. Run Python + SQL Notebook**

Open:

```
notebook/code.ipynb
```

Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn sqlalchemy
```

Run all cells to reproduce:
- SQL queries  
- EDA  
- Cleaning  
- Exporting cleaned dataset  

---

### **2. Open the Power BI Dashboard**

Download:

```
dashboard/Customer_behaviour_Dashboard.pbix
```

Open in Power BI Desktop → reconnect to:

```
data/cleaned/cleaned_customer_data.csv
```

---

## 📁 **Project Structure**

```
project/
│
├── data/
│   ├── raw/
│   │   └── customer_shopping_behavior.csv
│   └── cleaned/
│       └── cleaned_customer_data.csv
│
├── notebook/
│   └── code.ipynb
│
├── dashboard/
│   └── Customer_behaviour_Dashboard.pbix
│
├── images/
│   └── dashboard.png   (optional)
│
└── README.md
```

---

## 🙌 **Author**
**Dudala Vinay Kumar Goud**  
Data Analyst | Python | SQL | Power BI  

📧 Reach out for collaboration or feedback!



