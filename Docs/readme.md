
# Microsoft Fabric Data Engineering POC

## Project Overview

This project demonstrates an end-to-end Data Engineering solution using Microsoft Fabric.

The implementation follows Medallion Architecture:

Source System
      |
      |
Databag Layer
      |
      |
Bronze Layer
      |
      |
Silver Layer
      |
      |
Gold Layer
      |
      |
Power BI Reporting


## Technology Stack

| Component | Technology |
|---|---|
| Data Platform | Microsoft Fabric |
| Storage | OneLake |
| Processing | Fabric Notebooks (PySpark) |
| Orchestration | Fabric Data Pipelines |
| Data Warehouse | Fabric Warehouse |
| Reporting | Power BI |
| Version Control | GitHub |


## Project Phases

## Phase 1 - Requirement & Design

Completed:

- Repository setup
- Dataset analysis
- Data dictionary creation
- Data model design
- Source-to-target mapping
- Data quality assessment
- Business rule definition


## Repository Structure


docs/
- Project Overview
- Architecture
- Data Model
- ETL Design
- Incremental Load Design
- Audit Framework


datasets/
Sample source datasets


notebooks/
Fabric notebook implementations


pipelines/
Fabric pipeline JSON definitions


sql/
DDL and transformation scripts


powerbi/
Power BI reports

