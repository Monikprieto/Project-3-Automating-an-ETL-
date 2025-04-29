# Project-3-Automating-an-ETL-
Automating an ETL with Python: Automate data tasks.

Introduction
This project automates the process of preparing and loading customer support data into a PostgreSQL database using Python. It addresses the problem of inconsistent, manual data cleaning by building a functional ETL (Extract, Transform, Load) pipeline that prepares the dataset for analysis and reporting.

Dataset Description
The dataset used is `Customer_support_data.csv`, which contains over 85,000 records of customer service interactions. It includes:
- Contact channels and categories
- Timestamps for reported and resolved issues
- Agent and supervisor details
- Customer satisfaction (CSAT) scores
- Product and order-related fields

Some fields contain a high percentage of missing data and were handled or dropped during transformation.

Tools Used
- Python (pandas, datetime, sqlalchemy)
- PostgreSQL
- pgAdmin
- Jupyter Notebook
- Excel (for initial inspection)

Development Process

1.Extract
Data is read from a raw `.csv` file using `pandas`.

2.Transform
- Column names are normalized.
- Date fields are parsed and standardized.
- New metrics (e.g., response time) are calculated.
- Irrelevant or incomplete fields are removed.
- ETL load timestamp is added.

3. Load
Transformed data is loaded into a PostgreSQL table called `customer_support_cleaned` using SQLAlchemy.

Results and Conclusions
- A complete ETL pipeline was built and tested using real-world customer support data.
- The process ensures data consistency, type handling, and structure ready for analysis.
- Experience was gained in automating data workflows using Python and PostgreSQL integration.

This ETL pipeline serves as a reusable structure for automating future data loading and preprocessing tasks in customer service analytics.

Author
Monica Prieto — Data Engineer
