# Insurance Analytics Dashboard | Power BI

## Overview

This project is an interactive **Insurance Analytics Dashboard** built using Power BI.

It helps an insurance business track customers, revenue, policy performance, city-wise contribution, age-group behaviour, sales mode preference, and expected settlement exposure in one place.

The main purpose of this dashboard is to turn raw insurance data into clear insights that can support faster and better business decisions.

---

## Business Problem

Insurance teams need to track customer performance, premium revenue, policy movement, settlement exposure, and customer segments.

Without a single dashboard, it becomes difficult to answer important questions such as:

- How many customers do we have?
- Which city generates the highest revenue?
- Which age group contributes the most revenue?
- How are policy sales changing month over month?
- Which sales mode is preferred by customers?
- What is the expected settlement exposure?

This Power BI dashboard brings all these metrics together in an interactive report.

---

## Dashboard Pages

### 1. Insurance Performance Overview

This page provides a complete overview of insurance business performance.

Key features:

- Total Customers
- Total Revenue
- Daily Revenue Growth %
- Daily Customer Growth %
- Revenue and Customer Trend
- Policy Month-over-Month Growth
- City-wise Revenue Analysis
- Age Group-wise Revenue and Customer Analysis
- Interactive filters for City, Month, Age Group, Sales Mode, and Policy ID

### 2. Age Group Analysis

This page focuses on customer segmentation by age group.

Key features:

- Expected Settlement by Age Group
- Revenue by Age Group
- Customer Count by Age Group
- Sales Mode Preference
- Policy Preference
- Age Group Filters

---

## Data Model

The dashboard uses a star-schema-style data model with the following tables:

| Table | Description |
|---|---|
| `dim_customer` | Customer information such as customer ID, city, date of birth, and age group |
| `fact_premium` | Premium amount, policy purchase date, sales mode, and policy details |
| `dim_policy` | Policy details, base premium, and base coverage |
| `fact_settlement` | Settlement percentage and settlement-related information |
| `dim_date` | Date, month, year, and time-based analysis fields |

---

## Key DAX Measures

The following important measures were created:

- Total Customers
- Total Revenue
- Daily Revenue Growth %
- Daily Customer Growth %
- Policy MoM Growth %
- Expected Settlement
- Revenue by City
- Revenue by Age Group
- Customer Count by Age Group

### Expected Settlement Logic

    Expected Settlement =
    [Base Coverage] * [Settlement Percentage]

---

## Key Insights

- The dashboard tracks **26,841 customers** and approximately **₹989.3M total revenue**.
- **Delhi NCR** is the top revenue-generating city with around **₹401.6M revenue**.
- Delhi NCR contributes nearly **41% of total revenue**.
- **Mumbai** is the second-highest revenue-generating city.
- Revenue was highest in **March** and dropped in **April**.
- The **31–40 age group** is the strongest revenue-contributing customer segment.
- Expected settlement should be reviewed along with revenue and policy preference.

---

## Business Recommendations

- Protect Delhi NCR’s strong performance by analysing its sales channels and policy mix.
- Investigate the revenue drop from March to April.
- Create age-specific policy offers based on policy and sales mode preference.
- Focus on improving performance in lower-revenue cities.
- Monitor expected settlement exposure along with revenue growth.

---

## Tools Used

- Power BI
- Power Query
- DAX
- Data Modelling
- Excel / CSV

---

## Dashboard Preview

### Insurance Performance Overview

![Insurance Performance Overview](assets/insurance-overview.png)

### Age Group Analysis

![Age Group Analysis](assets/age-group-analysis.png)

> Upload your dashboard screenshots inside an `assets` folder with the same file names.

---

## Repository Structure

    Insurance-Analytics-Dashboard/
    │
    ├── Insurance Analytics Dashboard.pbix
    ├── Insurance Analytics Dashboard Presentation.pptx
    ├── Dataset/
    ├── assets/
    │   ├── insurance-overview.png
    │   └── age-group-analysis.png
    └── README.md

---

## Author

**Abhishek Singh Chauhan**  
Aspiring Data Analyst | Excel | SQL | Power BI | Business Reporting

[LinkedIn](YOUR_LINKEDIN_LINK) | [GitHub](YOUR_GITHUB_LINK)

---

If you found this project useful, please give this repository a star ⭐
