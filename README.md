# 🚀 Azure Data Engineering Projects

## 📖 Overview
This repository contains my **Azure Data Engineering** projects, showcasing my expertise in **Azure Data Factory (ADF), Azure Databricks, Azure SQL Database, Azure Data Lake Storage, and ETL pipelines**.

Each project demonstrates various **data integration, transformation, and processing** techniques used in real-world data engineering workflows.

---

## 📂 Projects Included

 
### **SCD Type 1 using Azure data factory**
**Project Level:** Beginner

**Description:** Developed a Slowly Changing Dimension (SCD) Type 1 pipeline using Azure Data Factory (ADF) to update customer records in an Azure SQL Database. The pipeline ensures that any changes in source data overwrite existing records without maintaining historical data.

**Tech Stack:** Azure Data Factory, Azure SQL Database, Azure Blob Storage.

**Key Features:**
1. Implemented SCD Type 1 logic to update records based on the latest source data.
2. Used Mapping Data Flow in ADF to perform UPSERT (Insert/Update) operations dynamically.
3. Integrated Azure Blob Storage for efficient data storage and retrieval.
4. Optimized pipeline performance by using Alter Row transformation for conditional updates.

➡️ **View Project**--> https://github.com/rrc0804/rrc-ade/blob/main/pl_SCD_Type1_proj.zip



### **Non-Empty File Copy using Azure Data Factory**  
**Project Level:** Beginner  

**Description:**  
Developed an Azure Data Factory (ADF) pipeline to automate the transfer of non-empty files from a source Azure Blob Storage container to a destination container. The pipeline ensures that only files containing data are copied, filtering out empty files to optimize storage and processing efficiency.  

**Tech Stack:**  
- Azure Data Factory  
- Azure Blob Storage  

**Key Features:**  
1. **Metadata Extraction:** Retrieves a list of files from the source container.  
2. **File Content Validation:** Uses a Lookup activity to check if the file contains data.  
3. **Conditional Processing:** Implements an `IfCondition` activity to allow copying only non-empty files.  
4. **Dynamic File Handling:** Uses a `ForEach` loop to process multiple files dynamically.  
5. **Optimized Data Transfer:** Ensures only meaningful data is transferred, reducing storage and compute costs.  

➡️ **View Project**-->https://github.com/rrc0804/rrc-ade/blob/main/pl_ADF%20Non-Empty_FileCopy.zip

**Website Breach Data Ingestion using Azure Data Factory**
**Project Level**: Beginner

**Description**:
Developed an Azure Data Factory (ADF) pipeline to ingest website breach data from a REST API and store it in Azure Blob Storage as structured text files. The pipeline extracts key information about website breaches, including breach date, affected domain, and security status, ensuring efficient data ingestion and storage for further analysis.

**Tech Stack**:

Azure Data Factory
REST API
Azure Blob Storage

**Key Features**:

1. Automated API Ingestion: Fetches website breach data using ADF's REST Source.
2. Pagination Handling: Supports RFC5988 pagination for retrieving large datasets efficiently.
3. Dynamic Data Mapping: Extracts multiple attributes, such as BreachDate, Domain, PwnCount, and IsVerified.
4. Structured Data Storage: Saves extracted data in Delimited Text format (.txt) within Azure Blob Storage.
5. Optimized Data Flow: Uses Tabular Translator to structure JSON API responses into tabular format.

➡️ **View Project**--> https://github.com/rrc0804/rrc-ade/blob/main/pl_ingest_website_breach_rest_api_data.zip


**Bulk Copy SQL Data to Azure Blob using Azure Data Factory**
**Project Level**: Intermediate

**Description**:
Developed an Azure Data Factory (ADF) pipeline to bulk copy tables from an Azure SQL Database to Azure Blob Storage in a structured text format. The pipeline dynamically retrieves table names from the database and iterates through each table to export its data into separate .txt files in the Blob storage.

**Tech Stack**:

Azure Data Factory
Azure SQL Database
Azure Blob Storage

**Key Features**:

1. Automated Table Discovery: Uses a Lookup activity to fetch all table names from information_schema.tables.
2. Dynamic Data Extraction: Uses a ForEach activity to iterate through tables dynamically.
3. Bulk Data Transfer: Efficiently copies all records from each table using the Copy activity.
4. Delimited Text Output: Stores data in CSV-like .txt files with headers in Azure Blob Storage.
5. Schema Flexibility: Supports multiple tables with different schemas using parameterized dataset references.

➡️ **View Project**--> https://github.com/rrc0804/rrc-ade/blob/main/pl_bulkcopy_SQL_to_blob.zip
