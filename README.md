🏦 Automated Credit Risk & Loan Portfolio Analytics Pipeline

📌 Project Overview

This project is an end-to-end automated data analytics pipeline designed to evaluate credit risk and analyze a large-scale loan portfolio.

The pipeline automates the extraction, transformation, and loading (ETL) of financial data and delivers an interactive Power BI dashboard for analyzing loan portfolio performance and credit risk.

The project demonstrates a complete analytics workflow, from raw financial data to actionable business insights using **Python, MySQL, and Power BI**.

---

🗄️ Data Source & Privacy Note

The dataset used in this project is the **Lending Club Loan Data (2007–2018)**.

The original dataset contains hundreds of thousands of financial records.

> **Note:** The raw CSV dataset is not included in this repository due to GitHub file-size limitations. The dataset can be obtained from the original public source on Kaggle:
> https://www.kaggle.com/datasets/wordsforthewise/lending-club

---

 🛠️ Tech Stack & Tools

| Category | Tools |
|---|---|
| Data Extraction & Transformation | Python, Pandas |
| Database Management | MySQL |
| Database Connectivity | SQLAlchemy, PyMySQL |
| Business Intelligence | Power BI |
| Data Visualization | Power BI |
| Workflow Automation | Windows Task Scheduler, Python Scripts |

---

 🚀 Key Features & Automation

### 1. Automated Python ETL Pipeline

Developed an optimized Python ETL pipeline using **Pandas** to process approximately **400k loan records** efficiently.

The pipeline uses:

- `chunking` to process data in manageable batches
- `usecols` to load only required columns
- Data cleaning and transformation
- Automated feature engineering

These techniques help reduce memory consumption and improve processing performance.

---

 2. Custom Risk Feature Engineering

Implemented business rules in Python to classify borrowers into:

- 🟢 **Low Risk**
- 🟡 **Medium Risk**
- 🔴 **High Risk**

The risk classification is based on borrower financial characteristics such as:

- Debt-to-Income (DTI) ratio
- Annual income

This feature allows the portfolio to be analyzed across different borrower risk segments.

---

 3. MySQL Database Integration

The transformed dataset is automatically loaded into a **MySQL database** using:

- SQLAlchemy
- PyMySQL

This creates a structured database layer that can be queried for further analysis and reporting.

---

 4. Power BI DirectQuery Integration

Power BI is connected to the MySQL database using **DirectQuery**.

This allows Power BI reports to query the underlying database directly instead of importing the complete dataset into the Power BI model.

The setup reduces the need for traditional data-import refreshes when querying updated database data.

---

 5. Interactive Financial Risk Dashboard

Built an executive-style Power BI dashboard focused on:

- Loan portfolio performance
- Default risk
- Borrower segmentation
- Credit grade analysis
- Loan purpose analysis
- Financial risk indicators

The dashboard enables users to interactively filter and explore portfolio performance.

---

 📊 Core Business Metrics Analyzed

 1. Defaulted Loan Value

Total monetary value of loans classified as **defaulted or charged off**.

---

2. Overall Default Rate

Percentage of loans classified as **defaulted or charged off** within the analyzed loan portfolio.

---

 3. Risk Segmentation

Analyzed loan performance and default rates across:

- Borrower risk categories
- Credit grades (A–G)
- Loan purposes

This helps identify segments with relatively higher or lower default risk.

---

4. Borrower Profiling

Analyzed relationships between borrower characteristics and loan outcomes, including:

- Annual income
- Debt-to-Income (DTI) ratio
- Home ownership
- Credit grade
- Loan purpose
- Default status

---

# 🔄 End-to-End Data Pipeline

```<https://github.com/Jay1912-pixel/Credit-Risk-Loan-Analytics-Pipeline>
Raw Lending Club CSV
        ↓
     Python
     Pandas
        ↓
Data Cleaning & Transformation
        ↓
Feature Engineering
        ↓
Risk Classification
        ↓
      MySQL
        ↓
    Power BI
   DirectQuery
        ↓
Interactive Risk Dashboard
        ↓
Business Insights
