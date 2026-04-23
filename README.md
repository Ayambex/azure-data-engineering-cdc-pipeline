# Azure Data Engineering CDC Pipeline

This project demonstrates an end-to-end data engineering pipeline built using Azure Data Factory.

## Architecture

The pipeline follows a medallion architecture:

- Raw Layer: Data ingestion from CDC API
- Curated Layer: Data transformation and cleaning
- Validation Layer: Data quality checks
- Analytics Layer: Aggregated insights

## Projects

### Project 1: Ingestion
- Ingested CDC data into Azure Data Lake (Raw layer)

### Project 2: Transformation
- Cleaned and transformed data using Data Flows
- Stored output in Curated layer (Parquet)

### Project 3: Validation
- Implemented data quality rules:
  - Null checks
  - Data type validation
  - Non-negative checks
- Used Conditional Split (First matching condition)
- Routed valid and invalid data accordingly

### Project 4: Analytics
- Aggregated data by state
- Generated summary dataset for reporting

## Tools Used

- Azure Data Factory
- Azure Data Lake Storage
- Parquet format
- Data Flows (Mapping Data Flow)

## Key Takeaways

- Built a scalable ETL pipeline using ADF
- Implemented data validation strategies
- Debugged real-world data pipeline issues
- Delivered analytics-ready data

