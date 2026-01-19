---
title: Data Profiling and Modelling for Tableau Vizualizations
date: 2025-12-01
links:
  - type: site
    url: https://github.com/rburris15/USFlights
  - type: dataset
    url: https://www.kaggle.com/datasets/shaivyac/us-airline-dataset

featured: true

tags:
  - Snowflake
  - Data Profiling
  - Data Normalization
  - Feature Creation
  - Data Modelling
---

This project demonstrates an end-to-end analytics engineering workflow using Snowflake to transform a raw, file-based dataset of US domestic flights into a clean, dimensional model optimized for business intelligence and visualization in Tableau.

Starting from a compressed flat file export, I designed and implemented a production-ready data pipeline that loads, profiles, cleans, and models flight transaction data within Snowflake. The final deliverable includes a normalized star schema with a central fact table, supporting dimension tables, and a business-friendly analytical view that abstracts technical complexity for downstream users.

**Key Objectives**

- Rapidly understand and profile unfamiliar, real-world transportation data

- Ingest and type raw file-based data using Snowflake staging and COPY INTO

- Design a dimensional data model aligned with BI best practices

- Address and document data quality issues encountered during transformation

- Expose analytics-ready features for business users and consultants

**What Was Built**

FACT_FLIGHTS: A transactional fact table containing flight-level measures and engineered analytical fields, including:

  - Distance banding (DISTANCEGROUP) for mileage-based analysis

  - Operational performance indicators such as departure delays over 15 minutes (DEPDELAYGT15)

  - Logical flags for next-day arrivals (NEXTDAYARR)

DIM_tables: Curated dimensions to support slicing and filtering, with cleaned airline and airport naming conventions to improve usability and readability

VW_FLIGHTS: A consolidated analytics view joining facts and dimensions, designed specifically for consumption by Tableau and non-technical stakeholders

**Data Quality & Modeling Considerations**

Identified and corrected obvious data inconsistencies where feasible (e.g., malformed names, timing edge cases)

Standardized text fields to remove embedded codes and concatenated metadata

Applied appropriate data typing and transformations to ensure accurate aggregations and time-based analysis

Preserved original column naming to meet automated validation and governance constraints

**Tools & Technologies**

  - Snowflake (staging, SQL transformations, dimensional modeling)

  - Cloud file ingestion via named stages

  - Tableau-oriented semantic modeling

  - SQL-based feature engineering and data validation

**Outcome**

The result is a clean, well-documented analytics layer that enables flight performance analysis by airline, route, distance band, and operational reliability—while demonstrating strong judgment in data modeling, quality handling, and stakeholder-oriented design.

This project reflects how I approach analytics engineering in consulting and production environments: balancing technical rigor, business usability, and clear communication of data limitations and assumptions.

<!--more-->
