# azure-databricsk-olympics-dataengineering-project
This is a demonstrator project wherein im using different Azure technologies to execute an end to end data engineering project.
## Steps Taken:
1. Setting up an Azure Account
2. Selecting a Data Source
3. Ingesting Raw Data to Azure Data Lake Gen 2 using Azure Data Factory.
4. Then transforming the Raw data using Spark in Azure Databricks.
5. Transfer the processed data to the Datalake.
6. Use Azure Synapse Analytics to process data to gain insights.
7. Create a PowerBI dashboard.

![Untitled Diagram](https://github.com/Gonsudev/azure-olympics/assets/34743726/a3c198b9-56f5-444f-9ec9-8fef7dfec53a)

## Services Used
![image](https://github.com/Gonsudev/azure-olympics/assets/34743726/85972cbd-5a26-4b24-b7f3-5777e3c4de04)

## Implementation
1. Creating a Datalake Gen2 storage account and then creating two containers for raw and ingested data.
   ![image](https://github.com/Gonsudev/azure-olympics/assets/34743726/8d267305-4f62-4587-b691-a83f2df47b03)
2. Ingesting Raw Data to Azure Data Lake Gen 2 using Azure Data Factory
   Create linked services, create pipelines, use copy data, select the source (web) and sink (Raw storage container in ADLS)
   ![image](https://github.com/Gonsudev/azure-olympics/assets/34743726/d567c803-68f1-4f32-a0d0-1beea9f8f212)
3. Create a new Azure Databricks application.
   * Create Compute : Where the actual nodes will run.
   * Create Notebook
   * Mount the Datalake to Databricks to access the files.
   * Create a connection between databricks and ADLS by going to Azure app registration and get the credentials, create a new secret key from Certificates and secrets panel.
   * Mount the datalake to databricks.
   * View and process the data using PySpark.
   ![image](https://github.com/Gonsudev/azure-olympics/assets/34743726/0ef51132-7301-4549-b400-3ea00d8e08c5)
4. Use Azure Synapse Analytics to understand the data more using SQL
   * Open Synapse studio
   * Data button : Contains data about data base tables and everything else
   * Develop : Used to create Notebook and SQL scripts and everything else.
   * Used Data to create a lake database.
   * Add tables.
     ![image](https://github.com/Gonsudev/azure-olympics/assets/34743726/ae9e554d-424b-4f24-97ea-3417d38810e8)
   * Go to develop -> SQL Script -> Start analysing and processing the data.
   * Once Processed, Connect to Power BI to create visualizations.



   

