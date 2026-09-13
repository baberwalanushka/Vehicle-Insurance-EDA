# 🚗 Vehicle Insurance Cross-Sell Analysis — EDA Project

> A beginner-friendly **Exploratory Data Analysis (EDA)** project that analyzes customer data to understand which existing health insurance customers are most likely to be interested in **vehicle insurance**.

---

## 📌 Objective

To explore customer demographics, vehicle history, and policy details in order to identify **patterns behind customer interest (Response)** in a vehicle insurance offer — using pure data analysis, **no Machine Learning**.

---

## 🛠️ Tools & Technologies

| Tool                                   | Purpose                      |
| -------------------------------------- | ---------------------------- |
| 🐍 **Python**                          | Data analysis                |
| 🐼 **Pandas**                          | Data cleaning & manipulation |
| 🔢 **NumPy**                           | Numerical operations         |
| 📊 **Matplotlib**                      | Data visualization           |
| 📈 **Seaborn**                         | Statistical visualization    |
| ☁️ **Google Colab / Jupyter Notebook** | Development environment      |

---

## 📂 Dataset

The dataset contains **381,109 rows × 12 columns**, with:

* 👤 **Customer Demographics:** Age, Gender, Region
* 🚗 **Vehicle Details:** Vehicle_Age, Vehicle_Damage
* 📋 **Policy Details:** Annual_Premium, Policy_Sales_Channel, Vintage
* 🎯 **Target Column:** `Response`

  * `1` = Interested
  * `0` = Not Interested


---

## 🧭 Project Workflow

```text
1. Data Understanding
        ↓
2. Data Cleaning
        ↓
3. Feature Engineering
        ↓
4. GroupBy Analysis
        ↓
5. Sorting & Filtering
        ↓
6. Data Visualization
        ↓
7. Business Insights
        ↓
8. Conclusion
```

### Step-by-Step

1. **Data Understanding**
   Shape, columns, data types, summary statistics

2. **Data Cleaning**
   Missing value check, duplicate removal

3. **Feature Engineering**
   Age_Group, Tenure_Group (time-based), Premium_Category

4. **GroupBy Analysis**
   Response rate across Gender, Age, Vehicle Age, Damage, Region, etc.

5. **Sorting & Filtering**
   Top premium customers, high-potential customer segments

6. **Visualization**
   15 charts built with Matplotlib & Seaborn

7. **Business Insights**
   10 key findings

8. **Conclusion**
   Summary of who to target and why

---

## 📊 Key Insights

### 🚗 Vehicle Damage

Customers with a **damaged vehicle** history respond at **~23.8%**, compared with just **~0.5%** for undamaged vehicles.

### 🛡️ Previous Insurance

Customers who are **already insured** almost never respond (**~0.09%**).

### 🚘 Vehicle Age

Customers with **vehicles older than 2 years** show the highest interest (**~29.4%**).

### 👥 Age Group

The **31–50 age group** is the most interested age segment (**~21%** response rate).

### ⏳ Customer Tenure

Customer **tenure (Vintage)** has almost no effect on response rate.

### 🎯 High-Potential Segment

A combined segment of **"damaged vehicle + not previously insured"** customers responds at **~25%** — nearly double the overall average.

---

## 👩‍💻 Author

### **Anushka Baberwal**

*Aspiring Data Analyst*

