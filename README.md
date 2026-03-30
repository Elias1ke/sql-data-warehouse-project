# sql-data-warehouse-project
Building a modern data warehouse with SQL, including ETL processes, data modelling and analytics.
 The project follows a structured Medallion Architecture, organizing data into bronze, silver, and gold layers to simulate professional engineering workflows. It covers the complete ETL (Extract, Transform, Load) process, including the ingestion of raw CSV files and the application of data cleansing and business logic. Beyond technical coding, the source emphasizes the role of a data architect by teaching data modeling, naming conventions, and the creation of project plans in Notion. 

How does Medallion architecture organize data into different layers?
Explain the role of ETL in modern data warehousing.
How do data engineers handle common data quality issues?
Today • 10:05 PM
write me a summary to include in read me github file

This project demonstrates the end-to-end development of a modern SQL Data Warehouse from scratch, implementing real-world industry standards and best practices
. The project covers the entire data engineering lifecycle, including data architecture design, ETL/ELT processing, data modeling, and documentation
.
Project Overview
The primary objective of this project is to build a centralized data management system using SQL Server to consolidate sales data from multiple sources (CRM and ERP systems)
. By transforming raw data into a structured format, the warehouse enables analytical reporting and informed business decision-making

Data Architecture
The warehouse follows the Medallion Architecture, which organizes data into three distinct layers to ensure quality and traceability
:
Bronze Layer (Raw): This layer stores unprocessed data exactly as it is received from the source systems (CSV files)
. It serves as the "landing zone" for data ingestion, ensuring a raw record is preserved for debugging and auditing
.
Silver Layer (Cleaned & Standardized): In this layer, the data undergoes heavy cleansing and standardization
. Key transformations include removing duplicates, handling missing values, casting data types, and normalizing coded values into user-friendly descriptions

Gold Layer (Business Ready): The final layer contains business-ready data modeled into a Star Schema
. It integrates multiple sources into optimized Fact and Dimension tables, featuring surrogate keys and calculated metrics designed specifically for reporting and BI tools

Key Features & ETL Process
ETL Implementation: Developed modular Stored Procedures to automate the Extract, Transform, and Load (ETL) process between layers
.
Data Modeling: Implemented a Star Schema consisting of dimensions (e.g., Customers, Products) and facts (e.g., Sales Transactions) to facilitate efficient querying
.
Data Quality & Validation: Built rigorous quality check scripts to identify issues such as unwanted spaces, invalid date ranges, and calculation inconsistencies
.
Advanced SQL Techniques: Utilized window functions (e.g., ROW_NUMBER, LEAD), complex CASE logic for data integration, and bulk inserts for high-performance loading
.
Technical Stack
Database: SQL Server (SQL Server Express)
Environment: SQL Server Management Studio (SSMS)
Documentation & Design: Draw.io (Data Flow and Integration Diagrams) and Notion (Project Management)
Version Control: GitHub
Project Documentation
This repository includes detailed documentation to support users and developers, including:
Data Flow Diagrams: Visualizing the lineage from source to the gold layer
.
Data Integration Model: Mapping relationships between source entities
.
Logical Data Model: Defining the Star Schema structure for the gold layer
.
Data Catalog: Comprehensive descriptions of all business objects and columns
