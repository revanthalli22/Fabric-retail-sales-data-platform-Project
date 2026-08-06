# Solution Architecture


## Architecture Overview


Source Systems

↓

Databag Layer

↓

Bronze Lakehouse

↓

Silver Lakehouse

↓

Gold Warehouse

↓

Power BI


## Microsoft Fabric Components


| Component | Purpose |
|-|-|
| Lakehouse | Storage and processing |
| Notebook | Transformation logic |
| Data Pipeline | Orchestration |
| Warehouse | Analytical model |
| Power BI | Visualization |


## Medallion Architecture


## Bronze Layer

Purpose:

- Store raw source data
- Preserve original format
- Minimal transformation


## Silver Layer

Purpose:

- Data cleansing
- Standardization
- Data validation
- Business transformations


## Gold Layer

Purpose:

- Business aggregates
- Star schema model
- Reporting datasets


## Data Flow


Source → Pipeline → Notebook → Lakehouse → Warehouse → Power BI
