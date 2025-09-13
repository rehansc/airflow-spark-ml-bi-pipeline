# 🚀 Airflow + Spark + ML + Power BI Pipeline

## 📌 Project Overview
This project demonstrates an **end-to-end data pipeline** combining:
- **Data Engineering**: Orchestration with Apache Airflow, scalable data processing with Apache Spark.  
- **Machine Learning**: Automated model training and evaluation.  
- **Business Intelligence**: Interactive dashboards with Power BI.  

Designed as a **portfolio showcase** for Data Engineering + ML + BI skills.

---

## 🏗️ Architecture
```mermaid
flowchart LR
    A[Raw CSV Data] -->|Ingest| B[Airflow DAG]
    B --> C[Data Processing - Pandas/Spark]
    C --> D[ML Training - scikit-learn/Spark MLlib]
    D --> E[Postgres - Data Warehouse]
    E --> F[Power BI Dashboard]
    
    subgraph Orchestration
        B
    end
    
    subgraph Processing
        C
        D
    end
    
    subgraph Storage & BI
        E
        F
    end
```
##⚡ Features

Data Ingestion

Load raw CSVs into the pipeline.

Process data with Pandas or Apache Spark.

Machine Learning

Train models (e.g., Logistic Regression).

Store metrics and results in Postgres.

Data Warehouse

Postgres stores processed data + ML outputs.

BI Dashboard

Power BI connects to Postgres for insights.

Orchestration

Airflow manages ETL, Spark jobs, and ML workflows.
