# Audit Framework


## Objective

Track pipeline execution, data movement, and failures.


## Audit Information Captured


| Field | Description |
|-|-|
| Pipeline_Name | Executed pipeline |
| Start_Time | Execution start |
| End_Time | Execution completion |
| Status | Success/Failure |
| Source_Count | Records extracted |
| Target_Count | Records loaded |
| Error_Message | Failure details |


## Logging Framework


Every pipeline execution generates audit records.


## Data Quality Checks


Checks performed:

- Null validation
- Duplicate validation
- Data type validation
- Referential integrity
- Record count validation


## Monitoring


Monitoring components:

- Fabric Monitoring Hub
- Pipeline Run History
- Notebook Logs
