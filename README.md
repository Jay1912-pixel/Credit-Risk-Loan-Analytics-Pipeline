# 🏦 Automated Credit Risk & Loan Portfolio Analytics Pipeline


 📌 Project Overview
This project is an end-to-end automated data analytics pipeline designed to evaluate credit risk and manage a large-scale loan portfolio. It automates the extraction, transformation, and loading (ETL) of financial data, culminating in a dynamic, enterprise-grade Power BI dashboard for executive decision-making.

The project demonstrates a complete data engineering and analytics workflow: moving from raw CSV data to actionable business intelligence using **Python, MySQL, and Power BI**.

 🗄️ Data Source & Privacy Note
The dataset used for this project is the **Lending Club Loan Data (2007-2018)**, comprising hundreds of thousands of financial records. 

*Note: Due to GitHub's file size limits and enterprise data privacy best practices, the raw CSV dataset is not uploaded to this repository. You can access the original public dataset directly from [Kaggle](https://www.kaggle.com/datasets/wordsforthewise/lending-club).*

 🛠️ Tech Stack & Tools
*   **Data Extraction & Transformation:** Python (Pandas)
*   **Database Management & Loading:** MySQL, SQLAlchemy, PyMySQL
*   **Business Intelligence & Visualization:** Power BI (DirectQuery mode)
*   **Workflow Automation:** Windows Task Scheduler / Python Scripts

 🚀 Key Features & Automation
*   **Automated Python ETL Pipeline:** Developed a highly optimized Python script to process a massive dataset. Utilized `chunking` and `usecols` to prevent memory overload, successfully processing and cleaning ~400k records in under 20 seconds.
*   **Custom Feature Engineering:** Implemented programmatic business logic in Python to classify borrowers into `High`, `Medium`, and `Low` risk categories based on their Debt-to-Income (DTI) ratio and Annual Income.
*   **Seamless Database Integration:** Automated the data loading process directly into a local MySQL database using SQLAlchemy, ensuring the data is structured and ready for enterprise querying.
*   **Live Power BI Connection:** Connected Power BI to the MySQL database via **DirectQuery**, allowing the dashboard to reflect real-time changes and updates without any manual data refreshes.
*   **Enterprise-Grade Dashboarding:** Re-engineered a premium "Dark Ruby" executive template into a focused financial dashboard highlighting critical risk KPIs.

 📊 Core Business Metrics Analyzed
1.  **Total Value at Risk (TVaR):** The total monetary value of loans that have defaulted or charged off.
2.  **Overall Default Rate:** The percentage of the loan portfolio that has failed to repay.
3.  **Risk Segmentation:** Analyzing default rates across varying credit grades (A-G) and loan purposes.
4.  **Borrower Profiling:** Understanding the correlation between annual income, debt-to-income (DTI), home ownership, and loan default probability.

 📁 Repository Structure
*   `etl_pipeline.py`: The Python script responsible for data extraction, cleaning, custom risk categorization, and MySQL database loading.
*   `Dashboard.pbix`: The final interactive Power BI dashboard file.
*   `Dashboard_Preview.png`: High-resolution screenshot of the Power BI dashboard.

💡 How to Run the Pipeline
1. Clone this repository to your local machine.
2. Ensure MySQL is running locally and update the database connection string in the Python script.
3. Run the ETL pipeline: `python etl_pipeline.py`
4. Open the Power BI file, refresh the DirectQuery connection, and view the updated metrics.
