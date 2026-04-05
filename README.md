# 📊 market-intelligence-core

A comprehensive Data Warehousing and Analytics solution built using **SQL Server**. This project demonstrates an end-to-end pipeline—from raw data ingestion to generating strategic business insights—following industry-standard engineering practices.

---

## 🏗️ Data Architecture: The Medallion Approach
This project implements a **Medallion Architecture**, ensuring data quality and structure as it moves through the pipeline:

* **🥉 Bronze Layer:** Ingests raw data as-is from source systems (ERP and CRM) into the SQL Server environment.
* **🥈 Silver Layer:** Focuses on data cleansing, standardization, and normalization, resolving quality issues to prepare data for modeling.
* **🥇 Gold Layer:** The "Source of Truth." Data is modeled into a **Star Schema** (Fact and Dimension tables) optimized for high-performance reporting.



---

## 📖 Project Objectives

### 1. Data Engineering (The Warehouse)
* **Objective:** Develop a modern data warehouse to consolidate fragmented sales data.
* **Integration:** Merged disparate data from ERP and CRM systems into a single, unified data model.
* **Quality:** Implemented robust cleansing logic to ensure data integrity for business stakeholders.

### 2. Data Analytics (The Insights)
* **Objective:** Develop SQL-based analytics to empower stakeholders with key metrics.
* **Focus Areas:** Customer behavior patterns, Product lifecycle performance, and Sales trend analysis.

---

## 📂 Repository Structure

```text
market-intelligence-core/
├── datasets/               # Raw ERP/CRM data (CSV) & Database Backups (.bak)
├── docs/                   # Architecture diagrams (ETL, Data Flow, Star Schema)
├── scripts/                # SQL Transformation Pipeline
│   ├── bronze/             # Extraction and raw loading scripts
│   ├── silver/             # Data cleaning and standardization logic
│   ├── gold/               # Final analytical modeling (Fact/Dim tables)
│   └── analysis/           # Advanced business logic (Scripts 05-13)
├── tests/                  # Data quality and validation scripts
└── README.md               # Project documentation

## 🛡️ License

This project is licensed under the [MIT License](LICENSE).