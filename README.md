# azure-population-pipeline
## Project Overview
A data engineering pipeline built using Azure cloud services that processes 
population data of the Top 100 World's Largest Cities using the 
Medallion Architecture (Bronze → Silver → Gold).

## Architecture
- 🥉 **Bronze Layer** - Raw CSV data stored in Azure Data Lake Storage
- 🥈 **Silver Layer** - Cleaned and transformed data using PySpark
- 🥇 **Gold Layer** - Top 10 most populated cities ready for analysis

## Tech Stack
- Azure Databricks
- Azure Data Lake Storage (ADLS Gen2)
- PySpark
- Python

## Notebooks
- `bronze_to_silver` - Reads raw data, cleans and saves to Silver layer
- `silver_to_gold` - Reads Silver data, extracts Top 10 cities, saves to Gold layer
