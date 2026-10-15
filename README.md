Microsoft Fabric – End-to-End Data Engineering Project

Overview

This project demonstrates an end-to-end data engineering workflow using Microsoft Fabric, covering data ingestion, incremental loading, data quality, transformation, and analytics.

The solution combines API and Excel data sources and organizes data through a Medallion Architecture to support reliable and analytics-ready datasets.

Architecture

Sources → Bronze → Silver → Gold → Semantic Model → Power BI Report

- Bronze: Ingest raw data from API and Excel sources into a Lakehouse.
- Silver: Clean, standardize, validate, and transform the ingested data.
- Gold: Prepare curated datasets for analytics and reporting.
- Semantic Model & Reporting: Organize analytical data and deliver insights through reports.

Key Features

1. Data Ingestion

- Ingest data from API and Excel sources.
- Implement incremental loading patterns.
- Use a control table to manage ingestion state and track previously processed data.

2. Data Transformation

- Apply data cleaning and standardization.
- Organize data into Bronze, Silver, and Gold layers.
- Implement hash-based change detection and Slowly Changing Dimension Type 2 (SCD Type 2) concepts to track historical changes.

3. Data Quality & Validation

- Perform data profiling to understand data structure and quality.
- Apply data validation using Great Expectations.
- Identify data quality issues before downstream processing.

4. Pipeline Orchestration & Maintenance

- Use Microsoft Fabric Data Pipelines to orchestrate ingestion workflows.
- Implement retention and cleanup workflows to support data lifecycle management.

5. Analytics & Reporting

- Build a semantic model for analytical consumption.
- Develop reports to present insights from processed data.

Technologies Used

- Microsoft Fabric
- Fabric Lakehouse
- Fabric Notebooks
- Fabric Data Pipelines
- Python
- SQL
- Great Expectations
- Medallion Architecture
- Incremental Data Loading
- Hash-Based Change Detection
- SCD Type 2
- Semantic Models & Power BI Reporting

What I Learned

- Building multi-source data ingestion workflows.
- Managing incremental loads using control tables.
- Structuring data pipelines with the Medallion Architecture.
- Implementing data profiling and validation.
- Tracking historical changes using SCD Type 2 concepts.
- Orchestrating workflows and managing data retention.
- Preparing curated data for analytics and reporting.

Repository Structure

- "FromAPI_NB.Notebook" — API ingestion.
- "FromExcel_NB.Notebook" — Excel ingestion.
- "Data Profiling.Notebook" — Data profiling.
- "Data Validation_GX.Notebook" — Data quality validation.
- "silver_nb.Notebook" — Silver-layer processing.
- "GoldNB.Notebook" — Gold-layer processing.
- "data_ingest.DataPipeline" — Data ingestion orchestration.
- "PL_Retention_Cleanup.DataPipeline" — Retention and cleanup workflow.
- "SalesModel.SemanticModel" — Semantic model.
- "SalesReport.Report" — Reporting layer.


Author

Mariam Salah
