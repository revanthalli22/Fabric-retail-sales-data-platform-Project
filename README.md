# Fabric-retail-sales-data-platform-Project


## Project Overview

The **Fabric Retail Sales Data Platform** is an end-to-end Data Engineering solution built using **Microsoft Fabric**.

The objective of this project is to design and implement a scalable data platform that ingests retail sales data, processes it through a Medallion Architecture, applies data quality rules, performs transformations, and delivers business-ready analytical datasets for reporting and analytics.


## Business Objective

The project aims to:

- Build a centralized retail data platform
- Automate data ingestion and transformation processes
- Improve data quality and reliability
- Enable incremental data processing
- Create analytics-ready datasets
- Support business reporting using Power BI


# Solution Architecture


The solution follows Microsoft Fabric Medallion Architecture:



Source Systems
|
|
v
Databag Layer
|
|
v
Bronze Layer
|
|
v
Silver Layer
|
|
v
Gold Layer
|
|
v
Power BI Analytics



## Architecture Layers


### Databag Layer

Purpose:

- Store raw extracted files
- Maintain source data snapshot
- Preserve original data format


### Bronze Layer

Purpose:

- Store raw ingested data
- Maintain source structure
- Perform basic validation


### Silver Layer

Purpose:

- Clean and transform data
- Apply business rules
- Handle data quality issues
- Create trusted datasets


### Gold Layer

Purpose:

- Create business-ready models
- Implement star schema
- Provide analytical tables for reporting


# Technology Stack


| Component | Technology |
|---|---|
| Cloud Data Platform | Microsoft Fabric |
| Storage | OneLake |
| Data Processing | Fabric Spark / PySpark |
| Data Orchestration | Fabric Data Pipelines |
| Data Storage | Lakehouse |
| Data Modeling | Star Schema |
| Reporting | Power BI |
| Version Control | GitHub |



# Dataset Overview


The project uses retail sales datasets containing:


| Dataset | Description |
|---|---|
| Customer | Customer master information |
| Product | Product details |
| Store | Store information |
| Sales | Retail sales transactions |
| Inventory | Inventory details |
| Calendar | Date dimension information |



# Data Engineering Approach


## Data Ingestion

Source data is loaded into Fabric using Data Pipelines.

Process:


Source Files
|
|
Fabric Pipeline
|
|
Bronze Lakehouse



## Data Transformation

Transformation is performed using Fabric Notebooks.


Process:


Bronze Data
|
|
PySpark Transformation
|
|
Silver Tables



## Data Modeling

The Gold layer follows a Star Schema design.


Example:


          DIM_CUSTOMER
                |
                |

DIM_STORE--DIM_PRODUCT ---- FACT_SALES ---- DIM_DATE


# Data Quality Framework


The platform implements data quality checks:

- Completeness validation
- Duplicate detection
- Data type validation
- Referential integrity checks
- Record count validation
- Business rule validation


# Incremental Load Strategy


The project supports incremental loading using watermark-based processing.


Approach:


Read Previous Watermark

    |

Extract New / Modified Records

    |

Load Bronze

    |

Transform Silver

    |

Update Watermark



Benefits:

- Reduced processing time
- Optimized resource usage
- Scalable data processing




# Repository Structure

Fabric-retail-sales-data-platform-Project
│
├── docs
│ ├── 01_Project_Overview.md
│ ├── 02_Solution_Architecture.md
│ ├── 03_Data_Model.md
│ ├── 04_ETL_Design.md
│ ├── 05_Incremental_Load_Design.md
│ └── 06_Audit_Framework.md
│
├── datasets
│
├── notebooks
│
├── pipelines
│
├── sql
│
├── powerbi
│
├── images
│
└── README.md



# Development Standards


## Naming Convention

Bronze:


brz_<table_name>



Silver:


slv_<table_name>



Gold:


gld_<table_name>



## Code Management

Source code and Fabric artifacts are maintained using GitHub.


# Project Status


| Phase | Status |
|---|---|
| Requirement Analysis | Completed |
| Architecture Design | Completed |
| Data Modeling | Completed |
| ETL Design | Completed |
| Fabric Development | Pending |
| Reporting | Pending |


# Future Enhancements

Future improvements:

- Automated deployment using CI/CD
- Metadata-driven pipelines
- Advanced monitoring framework
- Data governance implementation
- Performance optimization


# Author
Alli Revanth
Data Engineering Fabric Project

Technology:
Microsoft Fabric | PySpark | Power BI | GitHub
