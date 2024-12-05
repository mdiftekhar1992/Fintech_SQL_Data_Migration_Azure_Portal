# Fintech_SQL_Data_Migration_Azure_Portal

Azure Pipeline Flow for Fintech SQL Data Migration
-Azure Services Used:
-Azure SQL Database: Storing historical financial data.
-Azure Data Lake Storage (ADLS): Hosting the Bronze, Silver, and Gold data layers.
-Azure Synapse Analytics: Managing data ingestion and orchestration.
-PySpark: Implementing transformation logic for data processing.
-Delta Tables: Enabling efficient querying and updates across layers.
-Python & SQL: Supporting data transformations and queries.

Pipeline Workflow:
1-Prepare Historical Data:
. Configure Azure SQL Database with historical tables containing raw data.
2-Data Ingestion to Bronze Layer:
. Use Azure Synapse pipelines to extract data dynamically from SQL Database.
. Store unprocessed raw data in ADLS under the Bronze Layer.
3-Transform Data to Silver Layer:
. Execute a PySpark notebook to clean and standardize the Bronze Layer data.
. Save the transformed data as Delta Tables in the Silver Layer.
4-Refine Data to Gold Layer:
. Run a PySpark notebook for business-specific transformations and aggregations.
. Store analytics-ready data in the Gold Layer as Delta Tables.
5-Automated Pipeline Execution:
. everage Azure Synapse to sequence and automate the execution of all steps.
![diagram-export-05-12-2024-17_34_36](https://github.com/user-attachments/assets/20905297-39a0-4f0d-8bf1-91070c51e5ba)

