# 🏦 Automated Credit Risk & Loan Portfolio Analytics Pipeline


## 📌 Project Overview
This project is an end-to-end data analytics pipeline designed to evaluate credit risk and manage a large-scale loan portfolio. It automates the extraction, transformation, and loading (ETL) of financial data and provides a dynamic, enterprise-grade Power BI dashboard for executive decision-making.

The project demonstrates a complete data workflow: moving from raw CSV data to actionable business intelligence using **Python, MySQL, and Power BI**.

## 🛠️ Tech Stack & Tools
*   **Data Extraction & Transformation:** Python (Pandas)
*   **Database Management & Loading:** MySQL, SQLAlchemy, PyMySQL
*   **Business Intelligence & Visualization:** Power BI (DirectQuery mode)
*   **Environment:** VS Code, MySQL Workbench

## 🚀 Key Features & Automation
*   **Automated Python ETL Pipeline:** Developed a highly optimized Python script to process a massive dataset (~2.2 Million rows). Used `chunking` and `usecols` to prevent memory overload and processed ~400k records in under 20 seconds.
*   **Custom Feature Engineering:** Implemented a programmatic business logic in Python to classify borrowers into `High`, `Medium`, and `Low` risk categories based on their Debt-to-Income (DTI) ratio and Annual Income.
*   **Seamless Database Integration:** Automated the data loading process directly into a local MySQL database using SQLAlchemy, ensuring the data is structured and ready for querying.
*   **Live Power BI Connection:** Connected Power BI to the MySQL database via `DirectQuery`, allowing the dashboard to reflect real-time changes without manual data refreshes.
*   **Enterprise-Grade Dashboarding:** Re-engineered a premium "Dark Ruby" procurement template into a focused financial dashboard highlighting critical KPIs like Total Value at Risk (TVaR) and Default Rates.

## 📊 Core Business Metrics Analyzed
1.  **Total Value at Risk (TVaR):** The total monetary value of loans that have defaulted or charged off.
2.  **Overall Default Rate:** The percentage of the portfolio that has failed to repay.
3.  **Risk Segmentation:** Analyzing default rates across varying credit grades (A-G) and loan purposes.
4.  **Borrower Profiling:** Understanding the correlation between employment length, home ownership, and loan default probability.

## 📁 Repository Structure
*   `etl_pipeline.py`: The Python script responsible for data cleaning, transformation, and database loading.
*   `risk_analytics_queries.sql`: Advanced SQL queries used for deep-dive portfolio analysis (Cohort analysis, moving averages, etc.).
*   `Credit_Risk_Dashboard.pbix`: The final interactive Power BI dashboard file.

## 💡 How to Run the Pipeline
1. Clone this repository to your local machine.
2. Ensure MySQL is running and update the database credentials in the Python script.
3. Run the ETL pipeline: `python etl_pipeline.py`
4. Open the Power BI file, refresh the DirectQuery connection, and view the updated metrics.
