# Customer Churn Analysis | Python & Exploratory Data Analysis

**Python • Pandas • NumPy • Matplotlib • Seaborn • Business Insights**

An end-to-end customer churn analysis project that explores telecom customer behaviour, identifies high-risk customer segments, and generates data-driven recommendations to improve customer retention.

The project analyzes **7,032 customer records** to understand churn patterns across contract types, customer tenure, monthly charges, senior citizen status, and internet service categories.

---

## 📑 Table of Contents

1. About This Project
2. Problem Statement
3. Business Questions
4. Project Objectives
5. Dataset Overview
6. Project Structure
7. Methodology
   - Data Loading and Inspection
   - Data Cleaning and Preprocessing
   - Exploratory Data Analysis
   - Business Analysis
8. Key Findings
9. Business Recommendations
10. Technical Specifications
11. How to Run the Project
12. Limitations
13. Skills Demonstrated
14. Author

---

## 1. About This Project

Customer churn is a major business challenge for subscription-based companies. When customers discontinue their services, businesses may lose recurring revenue and face additional costs to acquire new customers.

This project focuses on analyzing telecom customer data to understand customer churn behaviour and identify the factors associated with customer attrition.

Using Python and its data analysis libraries, I performed data cleaning, exploratory data analysis, statistical summaries, and data visualization to discover meaningful patterns.

**The project demonstrates:**

- Data cleaning and preprocessing using Pandas.
- Exploratory Data Analysis (EDA) to understand customer behaviour.
- Group-wise analysis to compare churn across customer segments.
- Statistical summaries and percentage calculations.
- Data visualization using Matplotlib and Seaborn.
- Business insight generation and actionable recommendations.

---

## 2. Problem Statement

Telecommunication companies often experience customer attrition, where existing customers discontinue their subscriptions.

However, understanding the overall churn rate alone is not sufficient to identify the reasons behind customer departures.

Businesses need to understand:

- Which customer segments have higher churn rates?
- Does contract type influence customer retention patterns?
- Are new customers more likely to leave?
- Is there a relationship between monthly charges and churn?
- Which customer groups should receive more attention?

This project uses exploratory data analysis to investigate these questions and identify customer segments with comparatively higher observed churn.

---

## 3. Business Questions

The analysis focuses on the following business questions:

| No. | Business Question |
|---|---|
| 01 | What is the overall customer churn rate and retention rate? |
| 02 | Which contract types have the highest customer churn? |
| 03 | How does customer tenure relate to churn behaviour? |
| 04 | Do monthly charges differ between churned and retained customers? |
| 05 | How does churn vary between senior and non-senior customers? |
| 06 | Which internet service categories show higher churn? |
| 07 | What customer segments should businesses focus on to improve retention? |

---

## 4. Project Objectives

- Understand the overall customer churn and retention distribution.
- Inspect and clean the telecom customer dataset.
- Identify missing values, blank strings, and duplicate records.
- Analyze churn patterns across contract types and tenure groups.
- Compare customer characteristics based on churn status.
- Explore relationships between numerical features.
- Generate meaningful business insights.
- Provide recommendations to support customer retention strategies.

---

## 5. Dataset Overview

The project uses the **Telco Customer Churn Dataset**, which contains customer demographic information, subscribed services, contract details, tenure, billing information, and churn status.

**Dataset Summary**

| Attribute | Details |
|---|---|
| Total Customer Records | 7,032 |
| Target Variable | Churn |
| Customer Type | Telecom Customers |
| Data Format | CSV |
| Analysis Type | Exploratory Data Analysis |
| Primary Tool | Python |

**Important Features**

| Feature | Description |
|---|---|
| customerID | Unique customer identifier |
| gender | Customer gender |
| SeniorCitizen | Senior citizen indicator |
| Partner | Whether customer has a partner |
| Dependents | Whether customer has dependents |
| tenure | Number of months with the company |
| Contract | Customer contract type |
| MonthlyCharges | Monthly subscription charges |
| TotalCharges | Total charges paid by customer |
| InternetService | Type of internet service |
| PaymentMethod | Customer payment method |
| Churn | Whether the customer left the company |

Dataset Source: Kaggle – Telco Customer Churn Dataset.

---

## 6. Project Structure

```text
customer_churn_analysis/
│
├── data/
│   └── WA_Fn-UseC_-Telco-Customer-Churn.csv
│
├── notebooks/
│   └── customer_churn_analysis.ipynb
│
├── outputs/
│
├── requirements.txt
│
└── README.md
```

---

## 7. Methodology

### 1. Data Loading and Inspection

The first step was loading the dataset using Pandas and understanding its structure.

The following activities were performed:

- Loaded the CSV dataset.
- Inspected the first and last records.
- Checked dataset dimensions.
- Reviewed column names and data types.
- Generated descriptive statistical summaries.
- Checked missing values and duplicate records.

### 2. Data Cleaning and Preprocessing

Data cleaning was performed to ensure the dataset was suitable for analysis.

Key activities:

- Checked for missing and blank values.
- Removed unnecessary whitespace from text columns.
- Converted blank strings into missing values.
- Converted TotalCharges into a numeric data type.
- Inspected and handled missing TotalCharges records.
- Rechecked the cleaned dataset.

### 3. Exploratory Data Analysis (EDA)

EDA was performed to understand customer behaviour and identify patterns across different customer segments.

**Analysis Areas**

| Analysis | Purpose |
|---|---|
| Churn Distribution | Understand churned vs retained customers |
| Contract Analysis | Compare churn across contract types |
| Tenure Analysis | Identify churn patterns across customer tenure |
| Monthly Charges | Compare charges by churn status |
| Senior Citizen Analysis | Explore churn across senior citizen groups |
| Internet Service Analysis | Compare churn across service categories |
| Correlation Analysis | Explore relationships between numerical variables |

Visualizations were created using Matplotlib and Seaborn to communicate analytical findings.

### 4. Business Analysis

After completing the exploratory analysis, key business metrics were calculated.

The main metrics included:

- Total customers.
- Churned customers.
- Retained customers.
- Overall churn rate.
- Retention rate.
- Contract-wise churn rate.
- Tenure-wise churn rate.

**Churn Rate Formula**

```python
churn_rate = (
    churned_customers / total_customers
) * 100
```

**Retention Rate Formula**

```python
retention_rate = (
    retained_customers / total_customers
) * 100
```

---

## 8. Key Findings

The analysis of 7,032 telecom customer records produced the following findings.

### 1. Overall Customer Churn

| Metric | Result |
|---|---:|
| Total Customers | 7,032 |
| Churned Customers | 1,869 |
| Overall Churn Rate | 26.58% |
| Retained Customers | 5,163 |
| Retention Rate | 73.42% |

**Business Interpretation:**

Approximately 26.58% of customers discontinued their services. This indicates a significant customer retention challenge for the business.

### 2. Contract Type Analysis

- Month-to-month customers recorded a churn rate of **42.71%**.
- This customer segment showed comparatively higher churn than customers with longer-term contracts.

**Business Interpretation:**

Customers with flexible monthly contracts may require additional attention from customer retention teams.

### 3. Customer Tenure Analysis

- Customers with 0–12 months of tenure recorded a churn rate of **47.68%**.
- Early-stage customers represent an important segment for retention analysis.

**Business Interpretation:**

The first year of the customer relationship appears to be an important period for improving customer experience and retention.

### 4. Customer Behaviour Analysis

The analysis also explored differences in churn across:

- Monthly charges.
- Senior citizen status.
- Internet service categories.
- Contract types.
- Customer tenure.

These comparisons help businesses understand how churn patterns differ across customer segments.

---

## 9. Business Recommendations

Based on the observed analytical findings, the following recommendations can be considered.

**1. Improve Customer Onboarding**

Focus on the first 12 months of the customer journey. Improve onboarding, customer support, and early engagement.

**2. Review Month-to-Month Contracts**

Investigate pricing, service quality, and customer feedback among month-to-month customers. Evaluate suitable long-term contract benefits.

**3. Develop Customer Retention Strategies**

Identify customers showing potential churn risk and evaluate targeted retention campaigns.

**4. Monitor Customer Segments**

Regularly track churn across contract types, tenure groups, and internet service categories.

**5. Make Data-Driven Decisions**

Use customer analytics to evaluate retention strategies and measure their effectiveness over time.

These recommendations are based on observed patterns and should be validated through further business analysis and controlled experiments.

---

## 10. Technical Specifications

| Component | Technology / Approach |
|---|---|
| Programming Language | Python |
| Data Manipulation | Pandas |
| Numerical Analysis | NumPy |
| Data Visualization | Matplotlib |
| Statistical Visualization | Seaborn |
| Development Environment | Jupyter Notebook |
| Data Source | CSV |
| Analysis Type | Exploratory Data Analysis |
| Output | Analytical findings and visualizations |

---

## 11. How to Run the Project

### Step 1: Clone the Repository

```bash
git clone https://github.com/mitesh256/customer_churn_analysis.git
```

```bash
cd customer_churn_analysis
```

### Step 2: Create a Virtual Environment

```bash
python -m venv .venv
```

Activate the environment on Windows:

```bash
.venv\Scripts\activate
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Launch Jupyter Notebook

```bash
jupyter notebook
```

### Step 5: Run the Analysis

Open:

```text
notebooks/customer_churn_analysis.ipynb
```

Run the notebook cells sequentially to reproduce the analysis.

---

## 12. Limitations

- The analysis is based on the available telecom customer dataset.
- The project focuses on exploratory and descriptive analysis.
- Observed relationships do not establish causal relationships.
- The analysis does not include a predictive machine learning model.
- Business recommendations require further validation using customer feedback and business experiments.

---

## 13. Skills Demonstrated

- Python Programming
- Data Cleaning and Preprocessing
- Pandas and NumPy
- Exploratory Data Analysis (EDA)
- Statistical Analysis
- Data Visualization
- Group-wise Analysis
- Percentage and KPI Calculations
- Business Insight Generation
- Analytical Problem Solving

---

## 14. Author

**Mitesh Suthar**

Aspiring Data Analyst | Python | SQL | Power BI | Data Analytics

- GitHub: https://github.com/mitesh256
- LinkedIn: https://linkedin.com/in/mitesh-suthar256cse2026

---

**Customer Churn Analysis Using Python**

*Turning raw customer data into meaningful business insights.*
