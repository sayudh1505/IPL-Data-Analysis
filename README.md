# IPL Data Pipeline with Apache Spark & Databricks  

## Overview  
This project demonstrates the design and implementation of a **data pipeline** for Indian Premier League (IPL) datasets using **Apache Spark** on **Databricks**. The pipeline integrates with **Amazon S3** for scalable storage, processes large datasets for transformations, validates processed results in **MySQL**, and generates **visualizations** to analyze player performance, match statistics, and trends.  

## Architecture  
1. **Data Ingestion**  
   - Raw IPL datasets (CSV) are stored in **Amazon S3**.  
   - Spark reads data directly from S3 into Databricks notebooks.  

2. **Data Processing**  
   - Performed using **Apache Spark** (PySpark).  
   - Steps include:  
     - Data cleaning (handling nulls, duplicates, schema enforcement).  
     - Feature engineering (e.g., calculating batting averages, strike rates, economy rates).  
     - Filtering and aggregations (e.g., per match, per season, per player).  

3. **Data Validation**  
   - Processed data is pushed into **MySQL** for validation.  
   - SQL queries are used to cross-check Spark outputs.  

4. **Visualization**  
   - Insights generated using:  
     - Databricks built-in visualization tools.  
     - Custom Python libraries (`matplotlib`, `seaborn`, `pandas`).  
   - Key dashboards include:  
     - Top players by runs and wickets.  
     - Match outcome trends.  
     - Player performance evolution over seasons.  

## Tech Stack  
- **Databricks** – Managed Spark environment  
- **Apache Spark (PySpark)** – Distributed data processing  
- **Amazon S3** – Data lake storage  
- **MySQL** – Data validation and querying  
- **Python (matplotlib, seaborn, pandas)** – Data visualization  




## Repository Structure  
