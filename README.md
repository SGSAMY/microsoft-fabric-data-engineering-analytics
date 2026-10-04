# Microsoft Fabric Travel Insurance Analytics

An end-to-end data engineering and analytics project built using **Microsoft Fabric**, demonstrating data ingestion, transformation, Lakehouse architecture, Delta tables, semantic modelling and Power BI reporting.

## Project Overview

This project demonstrates how travel insurance policy and claims data can be processed through a modern Microsoft Fabric analytics workflow.

The solution ingests raw travel insurance data into a Fabric Lakehouse, transforms and validates the data using PySpark, creates curated analytical tables using Delta Lake, and exposes the results through a semantic model and interactive Power BI report.

## Architecture

**Source Data → Fabric Data Factory Pipeline → OneLake / Lakehouse → PySpark Transformation → Delta Tables → Semantic Model → Power BI**

### Microsoft Fabric Components

- **Fabric Data Factory** – pipeline orchestration and data ingestion
- **OneLake** – centralised data storage
- **Fabric Lakehouse** – storage and management of analytical data
- **PySpark Notebook** – transformation and data quality processing
- **Delta Lake** – curated analytical tables
- **Semantic Model** – business measures and analytical layer
- **Power BI** – interactive reporting and visualisation

## Data Engineering Workflow

### 1. Data Ingestion
A Microsoft Fabric Data Factory pipeline was created to ingest the source travel insurance dataset into the Fabric Lakehouse.

### 2. Lakehouse Storage
The ingested data is stored in OneLake through the Fabric Lakehouse, providing a central location for the project's data.

### 3. Data Transformation
A Fabric notebook using PySpark transforms and prepares the raw data for analytics.

The transformation process includes data type handling, derived fields and preparation of policy and claims data for downstream analysis.

### 4. Curated Delta Tables
The transformed data is written into Delta tables for analytical consumption.

The project includes analytical tables such as:

- `gold_fact_policy`
- `gold_claim_summary`

### 5. Semantic Model
A Fabric semantic model provides the business layer used by the Power BI report.

Key measures include:

- Policy Count
- Total Premium
- Total Claims
- Claim Ratio
- Highest Risk Policy Type

### 6. Power BI Analytics

The final report provides analysis of:

- Premium by destination
- Claims distribution by destination
- Monthly premium vs claims trends
- Claim ratio by policy type
- Policy distribution by sales channel
- Overall policy, premium and claims KPIs

Interactive slicers allow analysis by policy type, sales channel and policy start date.

## Key Technologies

`Microsoft Fabric` `Fabric Data Factory` `OneLake` `Lakehouse` `PySpark` `Delta Lake` `DAX` `Power BI`

## Business Insights

The analytical layer enables comparison of premium income against claims, identification of higher-risk policy types, analysis of destination-level performance and monitoring of policy distribution across sales channels.

For example, the portfolio analysis identifies **Annual Multi-Trip** as the policy type with the highest claim ratio in the sample dataset.

## Project Purpose

This portfolio project was created to demonstrate practical implementation of an end-to-end Microsoft Fabric data engineering and analytics workflow, from ingestion and transformation through to semantic modelling and business intelligence.
