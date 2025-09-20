***🔹 Databricks-End-to-End-Project***\

This project demonstrates an end-to-end data engineering pipeline built on Azure Databricks. It covers the complete data lifecycle — from ingestion, transformation, and storage, to building curated datasets(fact and dimention table) for analytics and reporting.The project simulates a real-world scenario of processing raw transaction data into meaningful business insights.

***🔹 Tech Stack***

-Cloud Platform: Microsoft Azure\
-Compute: Databricks (Apache Spark)\
-Storage: Azure Data Lake Storage Gen2 (ADLS)\
-Workflow Orchestration: Databricks Workflows / Jobs\
-Data Formats:Parquet, Delta Lake\
-Visualization: Power BI / Databricks SQL

***🔹Medallion Architecture***

**🔹Data Ingestion (Bronze Layer)**

-Raw Retail sales transaction data (Parquet) ingested into ADLS.\
-Databricks Auto Loader used for incremental ingestion.

**🔹 Data Transformation (Silver Layer)**

-Data cleaning: handling nulls, duplicates, schema enforcement.\
-Used classes,fucntions to transform data\
-Data standardization: converting datatypes, normalizing categorical fields.\
-Business logic applied using PySpark (e.g., calculating discounted price , categorize customers based on city).

**🔹 Data Aggregation (Gold Layer)**

-Aggregated data prepared for analytics by buikding fact and dimention tables(sales by region, product category trends, monthly revenue).\
-Stored in Delta Lake format for efficient querying.

🔹 Orchestration & Automation

-Databricks Jobs/Workflows scheduled for daily runs.\
-Monitoring and logging enabled.\
-ETL pieline created to handle daily incoming data.

🔹 Consumption Layer

-Power BI / Databricks SQL connected to Gold tables.\
-Dashboards for Sales Trends, Top Customers, and Revenue KPIs.

🔹 Features Implemented

✅ Raw → Bronze → Silver → Gold Medallion Architecture\
✅ Schema enforcement & incremental loading with Delta Lake\
✅ Data quality checks (duplicate removal, null handling, schema validation)\
✅ Partitioning & optimization for query performance\
✅ Automated pipeline orchestration with Databricks Workflows


🔹 Business Outcomes
-Reduced manual data preparation effort by 80%.\
-Improved query performance using Delta Lake optimizations.\
-Delivered ready-to-use analytics datasets for downstream BI tools.

