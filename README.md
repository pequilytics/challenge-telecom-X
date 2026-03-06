# 📊 Customer churn intelligence — Telecom X

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.0%2B-orange.svg)](https://pandas.pydata.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-0.12-green.svg)](https://seaborn.pydata.org/)

## 🏷️ About the project
This project presents a comprehensive **Exploratory Data Analysis (EDA)** for **Telecom X**, focusing on identifying the root causes of customer turnover (Churn). 

The analysis moves beyond basic descriptive statistics by utilizing **Feature Engineering** and **Statistical Correlation** to uncover hidden patterns in customer behavior. The ultimate goal is to provide data-driven insights to support retention strategies and prepare the dataset for future Machine Learning models.

## 🎯 Objectives
* **Diagnose churn drivers:** identify why customers are leaving the company.
* **Analyze financial impact:** evaluate the relationship between monthly charges and evasion.
* **Evaluate "lock-in" effects:** measure how the depth of the service ecosystem affects loyalty.
* **Statistical validation:** use correlation matrices to validate business hypotheses.

## 🗂️ Dataset & ETL Process
The project involved a robust **ETL (Extract, Transform, Load)** workflow:
* **Data normalization:** flattened nested JSON structures into a clean relational format.
* **Feature engineering:** * created `Daily_Charges` to monitor micro-billing patterns.
    * Developed `Total_Services` to quantify the customer's ecosystem depth.
* **Data integrity:** resolved `FutureWarning` issues and handled data type conversions (strings to Floats/Integers) for accurate mathematical processing.

## 💡 Key insights

### 1. The "first year" critical window
* **Finding:** 50% of customers who churn leave within the first **10 months**.
* **Statistical Proof:** a strong negative correlation (**-0.35**) between `tenure` and `Churn` proves that long-term customers are much more stable.
<img width="1383" height="583" alt="tempodecasa" src="https://github.com/user-attachments/assets/10d71e84-fd5f-4600-82f1-02bcdd7bf82b" />


### 2. High-ticket risk profile
* **Finding:** churners have a significantly higher average monthly bill (**$74.44**) compared to retained customers (**$61.27**).
* **Insight:** high prices without perceived value or service stability are driving customers away.

### 3. Service ecosystem (the lock-in effect)
* **Finding:** customers with **5 or more services** have near-zero churn rates.
* **Strategy:** increasing service depth is the most effective way to create "barriers to exit."

### 4. Technical & payment friction
* **Finding:** **Fiber Optic** users show the highest volume of cancellations (1,297 cases).
* **Finding:** **Electronic Check** payments are associated with much higher churn than automatic credit card methods.

## 🧠 Strategic Recommendations
* **Loyalty incentives:** focus on converting "Month-to-Month" contracts to annual plans during the first 12 months of tenure.
* **Cross-selling:** offer value-added services (Security, Backup) to low-service users to increase ecosystem depth.
* **Payment optimization:** encourage a switch to automatic payment methods to reduce monthly decision friction.

## 🛠️ Technologies Used
* **Python 3.x**
* **Pandas:** Data cleaning and manipulation.
* **Seaborn & Matplotlib:** Advanced data visualization and heatmaps.
* **Google Colab / Jupyter:** Development environment.

♡‧₊˚✧

Developed by Débora Tavares

Sales Operations & Data Intelligence

[LinkedIn](https://www.linkedin.com/in/deborasiltavares/)
