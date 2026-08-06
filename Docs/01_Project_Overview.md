# Project Overview


## 1. Introduction

This project implements a modern data engineering platform using Microsoft Fabric.

The objective is to ingest source data, perform data transformation, maintain data quality, and provide analytical datasets for reporting.


## 2. Business Objective

The main objectives are:

- Centralize data from multiple source systems
- Build scalable ETL pipelines
- Implement incremental data processing
- Maintain historical data
- Provide trusted datasets for analytics


## 3. Project Scope


### In Scope

- Data ingestion
- Data transformation
- Data quality validation
- Data modelling
- Pipeline orchestration
- Reporting layer


### Out of Scope

- Real-time streaming
- Machine learning models
- External application development


## 4. Dataset Overview


| Dataset | Description |
|-|-|
| Customer | Customer master information |
| Product | Product details |
| Vehicle | Vehicle master |
| Driver | Driver information |
| Shipment | Shipment transactions |
| Invoice | Invoice transactions |


## 5. Architecture Approach

The solution follows Medallion Architecture:

Bronze:
Raw ingestion layer

Silver:
Cleaned and transformed layer

Gold:
Business-ready analytical layer
