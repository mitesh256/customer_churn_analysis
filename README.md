# Customer Churn Analysis Using Python

## Project Overview

Customer churn is an important business problem for subscription-based companies. This project analyzes customer data to understand churn patterns, compare customer groups, and identify opportunities to improve customer retention.

The analysis uses Python for data cleaning, exploratory data analysis (EDA), statistical summaries, and data visualization.

## Objectives

- Understand the overall customer churn and retention rates.
- Clean and inspect the customer dataset.
- Analyze churn across contract types and customer tenure groups.
- Compare monthly charges and customer characteristics by churn status.
- Explore churn patterns across internet service categories.
- Generate data-driven business insights and recommendations.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Project Structure

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
└── README.md
```

## Dataset

The project uses the Telco Customer Churn dataset, which contains customer information, subscribed services, contract types, tenure, charges, and churn status.

The dataset can be obtained from:

[Kaggle — Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

Place the downloaded CSV file inside the `data/` directory.

## Project Workflow

### 1. Data Loading and Inspection

- Load the CSV dataset using Pandas.
- Inspect rows, columns, data types, and summary statistics.
- Review missing values, blank strings, and duplicate records.

### 2. Data Cleaning

- Remove unnecessary whitespace from text values.
- Convert blank strings to missing values.
- Convert `TotalCharges` into a numeric data type.
- Inspect missing values and handle missing `TotalCharges` records.
- Recheck the cleaned dataset.

### 3. Exploratory Data Analysis

The notebook investigates:

- Overall customer churn distribution.
- Churn rate by contract type.
- Customer tenure by churn status.
- Monthly charges by churn status.
- Churn by senior citizen status.
- Churn by internet service type.
- Correlations between numerical features.

### 4. Business Analysis

The project calculates churn and retention rates and identifies customer groups with comparatively high observed churn rates.

## Key Findings

The current analysis produced the following results:

| Metric | Result |
|---|---:|
| Customers analyzed | 7,032 |
| Churned customers | 1,869 |
| Overall churn rate | 26.58% |
| Retention rate | 73.42% |
| Churn rate for month-to-month contracts | 42.71% |
| Churn rate for customers with 0–12 months tenure | 47.68% |

These figures are based on the current notebook analysis and should be recalculated if the dataset or cleaning process changes.

## Business Recommendations

1. **Improve early customer experience:** Investigate onboarding and support issues among customers in their first year.
2. **Study month-to-month contracts:** Examine pricing, service quality, and customer feedback to understand the higher observed churn rate.
3. **Monitor customer segments:** Track churn by tenure, contract type, and internet service.
4. **Test retention strategies:** Evaluate targeted retention offers through controlled experiments before assuming they will reduce churn.
5. **Use evidence-based decisions:** Treat observed relationships as associations, not proof of causation.

## How to Run the Project

### Step 1: Clone the repository

```bash
git clone https://github.com/mitesh256/customer_churn_analysis.git
cd customer_churn_analysis
```

### Step 2: Create a virtual environment

```bash
python -m venv .venv
```

Activate it on Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

### Step 3: Install dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Open Jupyter Notebook

```bash
jupyter notebook
```

Open `notebooks/customer_churn_analysis.ipynb` and run the cells in order.

## Limitations

- The analysis identifies patterns and associations; it does not establish causal relationships.
- Findings depend on the dataset and the data-cleaning decisions.
- Business recommendations are hypotheses that require further validation.

## Skills Demonstrated

- Python for data analysis
- Pandas and NumPy
- Data cleaning and preprocessing
- Exploratory data analysis
- Data visualization
- Group-wise analysis and percentage calculations
- Business insight generation

## Author

**Mitesh Suthar**

Data Analytics | Python | Exploratory Data Analysis
