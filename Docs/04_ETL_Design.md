# ETL Design


## ETL Flow


Extract

↓

Transform

↓

Load



## Extraction Process


Source data is extracted using:

- Fabric Data Pipeline
- Copy Activity


## Bronze Load


Process:

1. Read source data
2. Validate schema
3. Load into Bronze tables


Example:

Source:

dbo.Customer


Target:

bronze_customer



## Silver Transformation


Operations:

- Data cleaning
- Null handling
- Data type conversion
- Duplicate removal
- Standardization



## Gold Transformation


Operations:

- Aggregations
- Business calculations
- Reporting tables


## Error Handling

Failed records are captured separately.

Pipeline execution logs are maintained.
