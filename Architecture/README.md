# Architecture

This folder contains the high-level architecture of the CDC data pipeline.

## Flow

API → Raw → Curated → Validation → Analytics

## Description

- API: Source data from CDC
- Raw: Data ingested in JSON format
- Curated: Cleaned and transformed data (Parquet)
- Validation: Data quality checks applied
- Analytics: Aggregated data for reporting
