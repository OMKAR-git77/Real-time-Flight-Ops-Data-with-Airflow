# Real-time-Flight-Ops-Data-with-Airflow
End to End real time  Data Engineering project with Airflow

# Overview
This project implements an end-to-end real-time data engineering pipeline focused on flight operations. it leverages Apache Airflow to orchestrate data workflows, including ingestion, transformation, and loading of flight-related data in real time. Additionally, Power BI is integrated for data visualization, enabling interactive dashboards and insights into flight operations metrics suchs as origin_country, on_ground, velocity, icao24.

# Project Snapshot
<img width="1307" height="735" alt="Screenshot (194)" src="https://github.com/user-attachments/assets/47aa967e-1bdd-48c8-97d1-c9de8207fca8" />

# Key Features
• Real-Time Data Ingestion: Fetch and process live flight data from APIs or streams into the bronze layer.  

• Medallion Architecture:  
       - Bronze Layer: Stores raw, unprocessed data.  
       - Silver Layer: Applies cleaning, validation, and basic transformations.  
       - Gold Layer: Aggregates data for business intelligence, stored in Snowflake for optimized querying.  

• Workflow Orchestration: Use Airflow DAGs to schedule and manage ETL (Extract, Transform, Load) tasks across layers.  

• Data Processing: Clean, transform, and aggregate flight operations data using Python scripts.  

• Data Storage: Snowflake for the gold layer, enabling scalable querying.  

• Visualization: Interactive dashboards in Power BI connected directly to Snowflake for real-time insights into key metrics.  

• Containerization: Dockerized setup for easy deployment and scalability.  

• Modular Structure: Easily extendable for additional data sources or analytics.  

# Technologies Used
• Apache Airflow: For workflow orchestration and scheduling.  
• Python: Core language for scripts and data processing.  
• Docker: Containerization via docker-compose.yml for Airflow setup.  
• Snowflake: Cloud data warehouse for storing and querying gold layer data.  
• Power BI: For creating visualizations and dashboards from Snowflake data.  
• Other dependencies as listed in requirements.txt.  

# Acknowledgments
• Built with Apache Airflow for robust orchestration.  
• Utilizes medallion architecture for structured data layering.  
• Data warehousing powered by Snowflake.  
• Visualizations powered by Microsoft Power BI.  
• Inspired by real-world flight operations data engineering needs.  
• Data Source - https://openskynetwork.github.io/opensky-api/rest.html  
• Special thanks to data with jay for inspiration and reference through their project:  
https://github.com/Jay61616/flight-ops-airflow  
