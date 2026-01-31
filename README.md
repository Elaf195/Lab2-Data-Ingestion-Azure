# Lab2-Data-Ingestion-Azure
Elaf Marouf 60107174

In this lab, I implemented an end-to-end data ingestion and transformation pipeline using Microsoft Azure. The key technical milestones achieved include:
- Environment Setup: Configured an Azure Machine Learning workspace and compute instance for data processing.
- Data Cleaning & Preparation: Identified and resolved formatting issues in the Amazon Electronics metadata. I utilized a Python script to convert non-standard JSON (single-quoted) into a valid, line-delimited JSON format suitable for modern analytics tools.
- Cloud Data Ingestion: Leveraged Azure CLI and AzCopy to securely transfer large datasets from a local compute environment to Azure Data Lake Storage (Gen2) using Shared Access Signature (SAS) tokens.
- ETL Pipeline Development: Built an automated orchestration pipeline in Azure Data Factory (ADF). This included:
Creating Linked Services and Datasets to connect ADF to storage.
Implementing a Mapping Data Flow to transform raw Unix timestamps into human-readable years.
Optimizing storage by partitioning the final output in Parquet format by review_year.
- Automation: Configured a Schedule Trigger to demonstrate how the pipeline can be automated for recurring data ingestion tasks.
- Final Outcome: The raw, unstructured Amazon reviews data was successfully transformed into a structured, partitioned, and high-performance Parquet dataset, ready for downstream analytical queries and machine learning models

<img width="1576" height="661" alt="image" src="https://github.com/user-attachments/assets/bd521f5b-480d-4c0a-b091-d0b3068e7e15" />

<img width="1080" height="602" alt="image" src="https://github.com/user-attachments/assets/97793648-5d74-4778-b1d8-820fe292533c" />

<img width="1091" height="628" alt="image" src="https://github.com/user-attachments/assets/8aaa34c0-8adb-44a0-9954-dac454dc9000" />

<img width="1237" height="535" alt="image" src="https://github.com/user-attachments/assets/6802747e-9637-43e3-87c5-a4f4c82c273e" />
