# Databricks Weather Data Pipeline

An automated weather data pipeline built using Databricks, PySpark and the Open-Meteo API. The project follows the Medallion architecture to ingest and transform weather data through Bronze, Silver and Gold layers.

## Architecture

Open-Meteo API → Bronze → Silver → Gold

## Technologies Used

- Databricks
- Python
- PySpark
- Delta Lake
- Open-Meteo API
- GitHub

## Pipeline Overview

### 1. Data Ingestion (Bronze)

Weather data is fetched from the Open-Meteo API and stored in a Bronze Delta table in Databricks.

### 2. Data Transformation (Silver)

The Silver layer applies data type conversions and transformations to the ingested weather data.

### 3. Data Aggregation (Gold)

The Gold layer aggregates weather data by date, including average, minimum and maximum temperatures, humidity, rainfall and wind measurements.

## Orchestration

Databricks Jobs are used to run the ingestion and transformation tasks in sequence.

## Data Source

[Open-Meteo API](https://open-meteo.com/)

## Current Status

The Databricks job has completed successfully. Further data-quality validation, including reconciliation of Bronze and Silver row counts, remains to be done.

## Screenshots

### Databricks Job Execution
<img width="1363" height="641" alt="image" src="https://github.com/user-attachments/assets/b412c321-562e-4f0a-ac1e-c0f88f3276b7" />


### Medallion Architecture Tables
<img width="1350" height="628" alt="image" src="https://github.com/user-attachments/assets/5fb2a360-7888-44c8-b815-3f7ab27be0c7" />

