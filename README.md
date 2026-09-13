🚗 Vehicle Insurance Cross-Sell Analysis — EDA Project

A beginner-friendly Exploratory Data Analysis (EDA) project that analyzes customer data to understand which existing health insurance customers are most likely to be interested in vehicle insurance.

📌 Objective

To explore customer demographics, vehicle history, and policy details in order to identify patterns behind customer interest (Response) in a vehicle insurance offer — using pure data analysis, no Machine Learning.

🛠️ Tools & Technologies
Python
Pandas
NumPy
Matplotlib
Seaborn
Google Colab / Jupyter Notebook
📂 Dataset

The dataset contains 381,109 rows × 12 columns, with customer demographics (Age, Gender, Region), vehicle details (Vehicle_Age, Vehicle_Damage), policy details (Annual_Premium, Policy_Sales_Channel, Vintage), and the target column Response (1 = interested, 0 = not interested).


🧭 Project Workflow
Data Understanding — shape, columns, data types, summary statistics
Data Cleaning — missing value check, duplicate removal
Feature Engineering — Age_Group, Tenure_Group (time-based), Premium_Category
GroupBy Analysis — response rate across Gender, Age, Vehicle Age, Damage, Region, etc.
Sorting & Filtering — top premium customers, high-potential customer segments
Visualization — 15 charts built with Matplotlib & Seaborn
Business Insights — 10 key findings
Conclusion — summary of who to target and why

📊 Key Insights
Customers with a damaged vehicle history respond at ~23.8%, vs just ~0.5% for undamaged vehicles.
Customers who are already insured almost never respond (~0.09%).
Customers with vehicles older than 2 years show the highest interest (~29.4%).
The 31–50 age group is the most interested age segment (~21% response rate).
Customer tenure (Vintage) has almost no effect on response rate.
A combined segment of "damaged vehicle + not previously insured" customers responds at ~25% — nearly double the overall average.
