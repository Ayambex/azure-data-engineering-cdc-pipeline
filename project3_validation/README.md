# Project 3: Data Validation

This phase focuses on validating and preparing CDC data for analytics using Azure Data Factory Data Flows.

## Objective
Ensure data quality by applying validation rules before moving data to the analytics layer.

## Validation Logic

The following checks were implemented:

- Non-null validation:
  - state
  - date
  - cases
  - deaths

- Data type conversion:
  - Converted cases and deaths from string to integer

- Range validation:
  - cases >= 0
  - deaths >= 0

## Conditional Split

A Conditional Split transformation was used with:

- **First matching condition**

This ensures:
- Valid records are routed to the **validated dataset**
- Invalid records are routed to the **validation_errors dataset**

## Output

- Valid data → `curated/validated/cdc`
- Invalid data → `curated/validation_errors/cdc`

## Result

After applying validation rules:
- All records passed validation
- No invalid records were generated

## Screenshots

### Validation Pipeline
![Validation Pipeline](validation_pipeline.png)

### Validation Result
![Validation Success](validation_success.png)
