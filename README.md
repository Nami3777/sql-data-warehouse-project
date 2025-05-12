# Data Warehouse & Analytics Portfolio Project

This project showcases a complete data warehousing and analytics pipeline—from raw data ingestion to delivering actionable business insights. Built as a portfolio project, it reflects best practices in data engineering, ETL design, and SQL-based reporting.

---

## 🏗️ Data Architecture: Medallion Layered Design

The project implements a **Medallion Architecture** approach consisting of three distinct layers to manage and optimize data flow:

| Layer       | Description                                                                 |
|-------------|-----------------------------------------------------------------------------|
| **Bronze**  | Raw data ingestion layer. CSV files from CRM and ERP systems are loaded into a SQL Server database with no transformation. |
| **Silver**  | Cleaned and standardized data. Here, inconsistencies are resolved, and data is normalized for structured analysis. |
| **Gold**    | Business-ready, analytics-optimized data. This layer uses a **star schema** to support efficient reporting and decision-making. |

---

## 📌 Project Scope

The project includes the following components:

- **Modern Data Architecture** using a layered approach (Bronze → Silver → Gold)
- **ETL Development**: Building pipelines to extract, transform, and load data
- **Data Modeling**: Designing fact and dimension tables for analytical performance
- **Analytical Insights**: Using SQL queries and dashboards to explore sales data

This project is ideal for demonstrating skills relevant to roles in:

- Data Engineering  
- Data Architecture  
- ETL Development  
- SQL Analytics  
- Business Intelligence  

---

## 📂 Project Requirements & Implementation

### Objective

Design and implement a centralized data warehouse in **SQL Server** for sales analytics using structured data from ERP and CRM systems.

### Specifications

- **Data Sources**: Two CSV files (ERP and CRM systems)
- **Data Quality Assurance**: Clean and standardize data for accuracy and usability
- **Data Integration**: Merge both systems into a cohesive, analytics-friendly model
- **Modeling Focus**: Implement a **non-historical**, current-state-only model
- **Documentation**: Include clear data model diagrams and field descriptions to support both business and technical users

---

## 📊 Analytics & Reporting

### Objective

Leverage SQL to uncover business-critical insights around:

- **Customer Segmentation & Behavior**
- **Top-Performing Products**
- **Seasonal & Trend-Based Sales Analysis**

These insights support strategic planning, performance monitoring, and data-driven decision-making.

---

## 📁 Repository Structure

```plaintext
data-warehouse-project/
│
├── datasets/                           # Raw datasets used for the project (ERP and CRM data)
│
├── docs/                               # Project documentation and architecture details
│   ├── etl.drawio                      # Draw.io file shows all different techniques and methods of ETL
│   ├── data_architecture.drawio        # Project’s overall data architecture
│   ├── data_catalog.md                 # Catalog of datasets, including field descriptions and metadata
│   ├── data_flow.drawio                # Diagram of end-to-end data flow
│   ├── data_models.drawio              # Star schema and data modeling structure
│   ├── naming-conventions.md           # Standardized naming rules for tables, fields, and scripts
│
├── scripts/                            # SQL scripts for ETL and transformations
│   ├── bronze/                         # Scripts for extracting and loading raw data
│   ├── silver/                         # Scripts for cleaning and transforming data
│   ├── gold/                           # Scripts for creating analytical models
│
├── tests/                              # Test scripts and quality validation checks
│
├── README.md                           # Project overview and instructions
├── LICENSE                             # License information for the repository
├── .gitignore                          # Files and directories to be ignored by Git
└── requirements.txt                    # Dependencies and requirements for the project

---


This project is licensed under the MIT License. You are free to use, modify, and share this project with proper attribution.
