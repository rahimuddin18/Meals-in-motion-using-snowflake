#  Meals in Motion: Swiggy-Inspired Data Pipeline in Snowflake

This project demonstrates an end-to-end data engineering pipeline inspired by Swiggy, built on **Snowflake**. It simulates the flow of food delivery data across multiple layers to support analytics and reporting.

---

##  Project Overview

- **Objective**: Design a modular pipeline for processing food delivery data using Snowflake.
- **Layers**:
  - **Stage Layer**: Ingest raw CSV data.
  - **Clean Layer**: Apply cleaning and basic transformations.
  - **Consumption Layer**: Build final tables for reporting and dashboards.
- **Tools**: Snowflake SQL, Snowsight, Streams & Tasks

---

## Data Sources

Sample transactional CSV files:


## Architecture

``plaintext
[Raw CSV Files]
      ↓
 Stage Tables (STG_)
      ↓ (via Streams & Tasks)
 Clean Tables (CLN_)
      ↓ (via Streams & Tasks)
 Consumption Tables (CNS_)
