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
