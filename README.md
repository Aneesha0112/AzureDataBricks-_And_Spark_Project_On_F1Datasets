# 🏎️ Real-World Formula 1 Data Engineering Project on Azure Databricks and Spark

This project demonstrates a **real-world, end-to-end data engineering pipeline** using **Azure Databricks**, leveraging **Formula 1 racing datasets** from 1950 to 2017. The solution follows the **Medallion architecture (Bronze → Silver → Gold layers)** and integrates key Azure services like **Data Lake Gen2**, **Azure Data Factory**, **Delta Lake**, **Unity Catalog**, **Azure Key Vault** and **Power BI**.

It showcases data ingestion, transformation, version control, and analytics — all built in a modern Lakehouse architecture optimized for scalability and governance.

---

## 👩‍💻 Author

**Aneesha Patan Arifulla**  
[📫 Email](mailto:sonyaneesha01@gmail.com) | [🔗 LinkedIn](https://www.linkedin.com/in/aneesha-patan/) | [💻 GitHub](https://github.com/Aneesha0112)

---

## 🔧 Project Architecture

- ✅ **Azure Data Lake Gen2** for scalable cloud storage  
- ✅ **Azure Databricks** for distributed processing using PySpark & Spark SQL  
- ✅ **Delta Lake** for ACID-compliant storage and time-travel  
- ✅ **Unity Catalog** for metadata management and data governance  
- ✅ **Azure Data Factory** for orchestration and scheduling  
- ✅ **Power BI** for reporting and visualization  

---

## 🗂️ Workflow Breakdown

### 1️⃣ Data Ingestion

- Ingested structured datasets (CSV/JSON) from Formula1 history (1950–2017)
- Data stored in **Bronze Layer** (Raw Zone) using Delta Lake format
- Incremental ingestion managed via **Azure Data Factory pipelines**

### 2️⃣ Data Transformation

- Transformed data using **PySpark** in Databricks notebooks
- Created **Silver Layer**: enriched, cleaned, and joined datasets
- Aggregated data (e.g., top drivers, fastest laps, championship points)
- Wrote final curated tables to **Gold Layer** for reporting

### 3️⃣ Data Governance

- Configured **Unity Catalog** to manage data access and lineage  
- Enabled **row-level access control** and audit features  
- Created structured namespace using catalogs, schemas, and tables

### 4️⃣ Time Travel & Optimization

- Enabled **Delta Lake time-travel** for data versioning and rollback
- Performed **VACUUM** and **OPTIMIZE** operations for performance tuning

### 5️⃣ Orchestration & Automation

- Designed ADF pipelines to trigger Databricks notebooks
- Parameterized pipelines for flexibility and scheduling
- Implemented error handling, retries, and pipeline dependencies

### 6️⃣ Visualization & Reporting

- Built interactive **Power BI dashboards**
- Connected directly to curated Delta tables using SQL endpoints
- Displayed insights like:
  - Most successful drivers/constructors
  - Lap time analysis
  - Race location heatmaps
  - Yearly performance comparisons

---

## 💡 Key Features

- ✅ **End-to-End Medallion Architecture** (Bronze → Silver → Gold)
- ✅ **PySpark and Spark SQL** transformations
- ✅ **Delta Lake ACID transactions** and time travel
- ✅ **Unity Catalog** for secure data governance
- ✅ **ADF pipeline orchestration**
- ✅ **Power BI integration** for real-time visualization

---

## 🧪 Sample Use Cases

- "What are the top 5 winning drivers each decade?"
- "Which race tracks produced the fastest laps over time?"
- "How did constructor performance evolve from 1950 to 2017?"
- "Track weather and lap time correlations (if extended with external APIs)"

---

## 📁 Repository Structure
[Folder Structure ](https://github.com/Aneesha0112/AzureDataBricks-_And_Spark_Project_On_F1Datasets/edit/main)
