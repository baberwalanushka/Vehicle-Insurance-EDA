# Project Report: Vehicle Insurance Cross-Sell Analysis

**Author:** Anushka Baberwal
**Type:** Exploratory Data Analysis (EDA)
**Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn

---

## 1. Introduction
Insurance companies often want to sell additional products to their existing customers — a practice known as **cross-selling**. In this project, an insurance company already has customers with **health insurance** and wants to know which of them are likely to also want **vehicle insurance**. This report presents an Exploratory Data Analysis of customer data to uncover patterns behind customer interest.

## 2. Dataset Description
The dataset (`Vehicle_Insurance.csv`) contains **381,109 records** and **12 columns**:

- **Demographics:** Gender, Age, Region_Code
- **Vehicle details:** Vehicle_Age, Vehicle_Damage, Driving_License
- **Policy details:** Previously_Insured, Annual_Premium, Policy_Sales_Channel, Vintage
- **Target column:** Response (1 = interested in vehicle insurance, 0 = not interested)

No missing values or duplicate rows were found, so the dataset required minimal cleaning.

## 3. Methodology
The analysis followed a standard EDA workflow:

1. **Data understanding** — inspected shape, data types, and summary statistics.
2. **Data cleaning** — verified there were no missing values or duplicates.
3. **Feature engineering** — created three new columns to simplify analysis:
   - `Age_Group` (20–30, 31–40, 41–50, 51–60, 61+)
   - `Tenure_Group` (based on the `Vintage` column — days associated with the company — used as the time-based feature since the dataset has no calendar dates)
   - `Premium_Category` (Low / Medium / High)
4. **GroupBy analysis** — measured the response rate across each customer segment.
5. **Sorting & filtering** — identified top premium customers and high-potential customer segments.
6. **Visualization** — built 15 charts to visually confirm the patterns found.

## 4. Key Findings

| Factor | Finding |
|---|---|
| Vehicle Damage | Damaged-vehicle customers respond at ~23.8% vs ~0.5% for undamaged |
| Previously Insured | Already-insured customers respond at only ~0.09% |
| Vehicle Age | Vehicles older than 2 years respond at ~29.4%, vs ~4.4% for vehicles under 1 year |
| Age Group | 31–50 age group has the highest interest (~21%) |
| Gender | Males respond slightly more often (13.8%) than females (10.4%) |
| Tenure (Vintage) | Has almost no effect on response rate (stays ~12.3% across all groups) |
| Combined Segment | "Damaged + Not Previously Insured" customers respond at ~25% — nearly double the overall average |
| Region | A small number of regions (e.g. Region 28) hold a large customer base and above-average response rates |
| Correlation | Annual Premium and Vintage show very weak correlation with Response |

## 5. Business Insights
1. Overall response rate across all customers is only about **12.3%**.
2. **Vehicle damage history** is the single strongest indicator of interest.
3. Customers who **already have insurance** should generally be excluded from vehicle insurance campaigns.
4. **Older vehicles** and the **31–50 age group** represent the best-fit customer profile.
5. **Tenure with the company does not predict interest** — new and long-standing customers behave similarly.
6. Combining "damaged vehicle" and "not previously insured" identifies a **high-value, easy-to-target segment**.
7. A few regions contribute disproportionately to both customer volume and response rate, useful for regional campaign planning.
8. Premium amount alone is not a strong predictor of interest.
9. Male customers show marginally higher interest than female customers.
10. The youngest age group (20–30) is the **least interested**, likely due to lower vehicle ownership or risk awareness.

## 6. Conclusion
This project demonstrates that simple, well-structured EDA — without any Machine Learning — can reveal clear, actionable customer segments. Customers with a **history of vehicle damage**, **no existing insurance**, an **older vehicle**, and an **age between 31–50** are the strongest candidates for a vehicle insurance cross-sell campaign. These findings can help a sales or marketing team focus their efforts and budget more effectively.

---
*This report accompanies the notebook `Vehicle_Insurance_EDA.ipynb` and the dataset `Vehicle_Insurance.csv`.*
