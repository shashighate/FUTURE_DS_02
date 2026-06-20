# Customer Retention & Churn Analysis

## Overview

This project was completed as part of the **Data Science & Analytics Internship Program** by Future Interns.

The objective of this project is to analyze customer churn and retention patterns using the Telco Customer Churn Dataset. The analysis focuses on identifying factors that influence customer attrition, understanding retention trends, and providing actionable business recommendations to improve customer loyalty and reduce churn.

---

## Project Objective

The primary goals of this project are to:

* Analyze customer churn behavior
* Identify customer segments with higher churn rates
* Understand the impact of contract type, tenure, internet service, and payment methods on retention
* Discover customer lifetime trends
* Provide business recommendations to improve customer retention

---

## Dataset

**Dataset Used:** Telco Customer Churn Dataset

Source:
https://www.kaggle.com/datasets/blastchar/telco-customer-churn

The dataset contains customer demographic information, subscription details, billing information, and churn status.

### Key Features

* Customer ID
* Gender
* Senior Citizen Status
* Tenure
* Monthly Charges
* Total Charges
* Contract Type
* Internet Service
* Payment Method
* Churn Status

---

## Tools Used

* Tableau
* Microsoft Excel (for initial data review)
* GitHub

---

## Data Cleaning & Preparation

The following preprocessing steps were performed:

1. Verified data types for all fields
2. Converted Total Charges to numeric format where required
3. Removed or handled missing values
4. Created calculated fields for churn analysis
5. Prepared data for visualization and KPI reporting

### Calculated Fields

**Churn Flag**

```text
IF [Churn] = "Yes" THEN 1 ELSE 0 END
```

**Retained Flag**

```text
IF [Churn] = "No" THEN 1 ELSE 0 END
```

**Churn Rate**

```text
SUM([Churn Flag]) / COUNT([customerID])
```

---

## Dashboard Components

### KPI Cards

* Total Customers
* Churned Customers
* Churn Rate (%)

### Visualizations

* Churn by Contract Type
* Churn by Internet Service
* Churn by Payment Method
* Churn by Tenure Group
* Churn by Gender
* Churn by Senior Citizen Status

### Interactive Filters

* Contract Type
* Gender
* Internet Service

---

## Analysis Performed

### Customer Churn Analysis

Analyzed overall customer churn levels to understand the percentage of customers leaving the service.

### Contract-Based Retention Analysis

Compared churn rates across different contract types to identify retention patterns.

### Tenure Analysis

Examined how customer lifetime impacts churn probability.

### Service-Based Analysis

Evaluated the relationship between internet service types and customer churn.

### Payment Behavior Analysis

Investigated whether payment methods influence customer retention.

### Customer Segmentation

Compared churn behavior across demographic groups such as gender and senior citizen status.

---

## Key Insights

### Churn Trends

A significant portion of churn originates from customers with shorter tenures, indicating that early customer engagement is critical.

### Contract Impact

Customers on month-to-month contracts tend to have higher churn rates compared to customers on long-term contracts.

### Service Impact

Internet service type plays an important role in customer retention and satisfaction.

### Payment Behavior

Certain payment methods show higher churn concentrations, suggesting opportunities for process improvements.

### Customer Lifetime

Longer-tenure customers are generally more loyal and less likely to churn.

---

## Business Recommendations

1. Encourage customers to move from month-to-month plans to longer-term contracts.
2. Strengthen onboarding and engagement during the first year of customer subscription.
3. Offer loyalty rewards for long-term customers.
4. Develop targeted retention campaigns for high-risk customer segments.
5. Improve customer support and service quality for segments with elevated churn rates.
6. Promote convenient automatic payment options to improve retention.

---

## Dashboard Preview

The dashboard provides an interactive view of customer retention metrics and churn drivers, enabling stakeholders to identify risk areas and make data-driven decisions.

---

## Project Structure

```text
FUTURE_DS_02
│
├── Dataset
│   └── Telco-Customer-Churn.csv
│
├── Tableau Dashboard
│   └── FUTURE_DS_02.twbx
│
├── Screenshots
│   └── dashboard.png
│
├── Report
│   └── Customer_Retention_Analysis.pdf
│
└── README.md
```

---

## Skills Demonstrated

* Data Cleaning and Preparation
* Customer Retention Analysis
* Churn Analysis
* Customer Segmentation
* KPI Development
* Data Visualization using Tableau
* Business Storytelling
* Insight Generation and Reporting

---

## Internship Information

**Internship:** Data Science & Analytics Internship

**Task:** Customer Retention & Churn Analysis (Task 2)

**Organization:** Future Interns

---

## Author

**Shashikant Ghate**

Data Science & Analytics Intern

Future Interns
