# 🏥 US Healthcare Claims Denials – Revenue Analytics Using Python

## 📌 Project Overview

This project analyzes US healthcare claims data to understand claim approval and rejection patterns, identify common rejection reasons, evaluate payer-level collection gaps, and examine payment turnaround performance.

Python is used for data cleaning, exploratory data analysis (EDA), statistical analysis, and visualization. Power BI is used to build interactive dashboards that present key performance indicators and business insights.

## 🎯 Business Problem

Healthcare organizations may experience claim rejections, delayed payments, incomplete documentation, and gaps between billed and collected amounts. These issues can affect revenue cycle efficiency and increase administrative rework.

This project uses historical claims data to identify recurring patterns and recommend practical improvements to claims processing and revenue collection.

## 🎯 Project Objectives

- Analyze claim approval, rejection, and pending status distributions.
- Identify the most common claim rejection reasons.
- Evaluate payer-level rejection patterns and collection gaps.
- Compare billed amounts with collected amounts.
- Analyze payment turnaround time and missing payment dates.
- Develop business recommendations to improve claim processing and revenue cycle performance.

## 📂 Dataset Information

- **Dataset:** Medical Billing RCM Dataset
- **Source:** Hugging Face
- **Original dataset size:** 100,000 rows and 30 columns
- **Dataset after cleaning:** 99,906 rows and 26 columns
- **Domain:** US Healthcare Revenue Cycle Management (RCM)

The dataset includes claim identifiers, submission dates, billed and collected amounts, approval status, rejection reasons, insurance company, claim type, service line, payment information, and other claim-related attributes.

## 🛠️ Tools and Technologies

- **Python** – Data analysis and exploratory analysis
- **Pandas and NumPy** – Data manipulation and numerical analysis
- **Matplotlib and Seaborn** – Data visualization
- **Google Colab / Jupyter Notebook** – Python development environment
- **Power BI** – Interactive dashboard development

## 🧹 Data Cleaning and Preparation

The following data preparation steps were performed:

- Reviewed the dataset structure and data types.
- Removed exact duplicate records, reducing the dataset from 100,000 to 99,906 rows.
- Removed four unnecessary columns, leaving 26 relevant columns.
- Standardized placeholder values in selected categorical fields.
- Identified missing final payment dates and payment turnaround values.
- Flagged negative billed amounts for review rather than automatically deleting potentially meaningful financial adjustments.
- Reviewed repeated BillingID values separately from exact duplicate records.

## 📊 Key Performance Indicators (KPIs)

| KPI | Result |
|---|---:|
| Total Claims | 99,906 |
| Total Billed Amount | 38.05M |
| Total Collected Amount | 17.63M |
| Collection Rate | 46.3% |
| Rejection Rate | 15.29% |
| Approved Claims | 73.78% |
| Rejected Claims | 15.29% |
| Pending Claims | 10.94% |
| Claims with Missing Final Payment Dates | 26.99% |

*Note: Amounts and percentages are based on dashboard results and may be rounded.*

## 🐍 Python Analysis

The Python notebook includes:

- Dataset overview and data quality checks
- Missing-value and duplicate analysis
- Claim status distribution analysis
- Rejection rate by insurance company
- Collection performance by payer
- Claim approval status by service line
- Top claim rejection reasons
- Descriptive statistics for numerical variables
- Payment turnaround time analysis
- Outlier analysis using box plots
- Billed amount versus payment turnaround analysis
- Correlation analysis and heatmap
- Pairplot analysis using a sample of the dataset

## 📈 Power BI Dashboard

The interactive Power BI dashboard contains five pages.

### 1. Executive Summary

Provides an overview of total claims, billed amount, collected amount, collection rate, rejection rate, claim status distribution, and monthly claim submission trends.

### 2. Revenue & Claims Analysis

Examines revenue performance, billed versus collected amounts by payer, and claim submission patterns.

### 3. Denial & Payer Deep Dive

Highlights major rejection reasons, payer-level rejection patterns, and collection gaps across insurance companies.

### 4. Denial Root Cause Analysis

Explores recurring rejection categories and claim-related patterns to identify areas that require further investigation.

### 5. Payment & Operational Insights

Analyzes payment turnaround trends and the availability of final payment dates.

## 🔍 Key Findings

- The overall claim rejection rate was approximately **15.29%**.
- Invalid Insurance was the leading displayed rejection reason, with approximately **3.04K claims**.
- Authorization Required and Missing Documentation each accounted for approximately **3.01K claims**.
- Incorrect Patient Info accounted for approximately **3.00K claims**.
- Procedure Not Covered accounted for approximately **2.95K claims**.
- The total billed amount was approximately **38.05M**, compared with **17.63M collected**.
- The overall collection rate was approximately **46.3%**.
- UnitedHealth showed the largest displayed collection gap at approximately **6.23M**, followed by Aetna at approximately **5.13M**.
- Approximately **26.99% of claims had missing final payment dates**.

## 💡 Business Recommendations

- Verify insurance eligibility and patient details before claim submission.
- Strengthen prior authorization tracking and documentation checks.
- Review common rejection reasons and implement preventive validation procedures.
- Prioritize outstanding claims based on claim age and unpaid amount.
- Investigate payer-specific collection gaps and payment delays.
- Improve the completeness and accuracy of final payment date records.
- Monitor rejection rate, collection rate, and payment turnaround regularly through Power BI.
- Provide targeted training on common rejection reasons and payer requirements.
- Explore predictive analytics in future work to identify claims at higher risk of rejection or payment delay.

These recommendations are proposed actions. Their actual impact should be evaluated after implementation by comparing performance over time.

## ✅ Conclusion

This project demonstrates how Python and Power BI can be combined to analyze healthcare claims and revenue cycle performance. The analysis identifies common rejection reasons, payer-level collection gaps, payment data completeness issues, and opportunities to improve claim processing.

The findings can support data-driven decision-making, help prioritize operational improvements, and guide efforts to reduce avoidable rejections and strengthen revenue collection.

```

## 👩‍💻 Author

**Hema Ishwarya C**

Healthcare RCM | Quality Assurance | Python | Power BI | SQL

[LinkedIn Profile](https://www.linkedin.com/in/hemaishwarya/)
