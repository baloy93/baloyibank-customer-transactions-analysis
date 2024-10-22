# baloyibank-customer-transactions-analysis

This project demonstrates a comprehensive data engineering pipeline designed to process and analyze customer transaction data. The pipeline leverages multiple Azure services to deliver an end-to-end solution, from data generation to advanced analytics and reporting. The key components of the project include data ingestion, storage, transformation, and visualization using tools such as Azure Data Lake Storage, Azure Data Factory, Azure Databricks, Azure Synapse Analytics, and Power BI.

Architecture Overview;
Data Generation: Synthetic customer transaction data is generated using a Python script within Jupyter Notebook.
Data Storage: Azure Data Lake Storage (ADLS) is utilized as the scalable, cloud-based storage solution for both raw and processed data.
Data Orchestration: Azure Data Factory (ADF) manages the ETL (Extract, Transform, Load) process by automating data movement and transformations between services.
Data Transformation: Azure Databricks, powered by Apache Spark, performs data transformation and enrichment tasks at scale.
Data Warehousing: Azure Synapse Analytics serves as the data warehouse, allowing for high-performance querying and analysis of the processed data.
Data Visualization: Power BI is used to create interactive reports and dashboards for data-driven insights.

Key Technologies Used;
Python (Jupyter Notebook): Used to generate synthetic transaction data and create reproducible datasets for analytics.
Azure Data Lake Storage (ADLS): Secure, highly scalable cloud storage solution for both structured and unstructured data.
Azure Data Factory (ADF): A fully managed ETL service for orchestrating data movement and transformation.
Azure Databricks: Apache Spark-based platform for large-scale data processing and machine learning.
Azure Synapse Analytics: Unified analytics platform for big data and data warehousing, allowing seamless integration with ADLS and Databricks.
Power BI: Business intelligence tool used to create interactive dashboards and visualizations for business analytics.

Pipeline Overview;
Data Generation:

Synthetic customer transaction data is generated using a Python script within Jupyter Notebook, simulating real-world customer transactions with attributes such as CustomerID, TransactionAmount, TransactionDate, MerchantCategory, and Location.
Data Ingestion and Storage:

The generated dataset is uploaded to Azure Data Lake Storage (ADLS), where both raw and processed data are stored in designated folders.
ETL Process using Azure Data Factory:

Azure Data Factory orchestrates the data flow by extracting the raw data from ADLS, transforming it using data flow pipelines, and loading the processed data back into a different folder in ADLS.
Data Transformation with Azure Databricks:

Further data processing and enrichment is conducted on Azure Databricks. Apache Spark is used to handle transformations, such as data cleaning, aggregation, and the generation of new features for analytics.
Data Warehousing with Azure Synapse Analytics:

The transformed data is loaded into Azure Synapse Analytics, which acts as the data warehouse. The data can be queried using T-SQL for analysis or integrated with other services for deeper insights.
Data Visualization with Power BI:

The processed data from Synapse Analytics is connected to Power BI for creating interactive dashboards. Visualizations include transaction trends over time, total transactions by category, and geographic heat maps of transaction locations. Filters and slicers allow users to dynamically explore the data.

Project Structure;
/Data: Contains the generated data files.
/Jupyter_Notebook: Includes the Python script used to generate synthetic customer transaction data.
/PowerBI_Dashboard: Contains Power BI reports and dashboards.
/Azure_Pipeline: Documentation on setting up and configuring Azure Data Lake, Data Factory, Databricks, and Synapse Analytics.
How to Use This Project
Clone the Repository: Clone this repository to your local machine.
Data Generation: Run the Python script provided in the /Jupyter_Notebook directory to generate the customer transaction dataset.

Azure Setup;
Azure Data Lake Storage: Set up an ADLS container to store raw and processed data.
Azure Data Factory: Create and configure data pipelines to automate data processing.
Azure Databricks: Use Databricks notebooks for data transformation tasks.
Azure Synapse Analytics: Load the transformed data into Synapse for querying.
Data Visualization: Connect Power BI to Synapse Analytics to visualize the processed data and build interactive dashboards.

Conclusion;
This project demonstrates the integration of key Azure services for building a scalable, cloud-based data engineering pipeline. It highlights how to automate data workflows, process large datasets, and deliver actionable insights through advanced analytics and visualizations. The end-to-end solution is designed to be highly scalable, robust, and easily extendable for future data projects.

note: Because I was using azure free subscription to do my projects, I excceded my aceess limits and was only to able access my notebooks uloaded.
