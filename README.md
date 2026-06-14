# SAP HANA 2.0 SPS 05 (XSA) – Case Study

## Overview
This repository contains my implementation of the SAP HANA 2.0 SPS 05 (XSA) case study provided by SAP UCC Munich.

The project demonstrates the development of data models and analytical views using SAP HANA XS Advanced (XSA) and SAP Web IDE.

## Objectives
- Understand SAP HANA XSA architecture
- Work with SAP Web IDE Development and Analysis tools
- Configure cross-container access
- Create HDI container connections
- Build calculation views for analytics
- Perform sales data analysis using SAP HANA

## Technologies Used
- SAP HANA 2.0 SPS 05 (XSA)
- SAP Web IDE
- HDI Containers
- HDBCDS Artifacts
- HDB Grants
- HDB Synonyms
- Calculation Views
- Star Schema Modeling

## Implemented Tasks

### Task 1: Cross-Container Access
- Created Multi-Target Application (MTA)
- Created Database Module
- Added SAP HANA Service Connection
- Configured `.hdbgrants`
- Created `.hdbsynonym` files
- Accessed external HDI container `hdi_GBI_DEMO`

### Task 2: Sales Organization Table
- Created `Salesorg` table using HDB CDS
- Imported `Salesorg.csv`
- Configured `.hdbtabledata`

### Task 3: Customer Dimension View
Created `CUSTOMER_XXX_DIM_CV` including:
- Customer data
- Country information
- Sales Organization information
- Text joins and filters

### Task 4: Product Dimension View
Created `PRODUCT_XXX_DIM_CV`:
- Included product attributes
- Excluded price information

### Task 5: Sales Cube
Created `SALES_XXX_CUBE_CV`:
- Cube with Star Join
- Customer and Product dimensions
- Calculated column:
  - `NET_REVENUE = REVENUE - DISCOUNT`

### Task 6: Ranking View
Created `SALES_RANK_XXX_CUBE_CV`:
- Filtered sales data for:
  - Country = Germany (DE)
  - Year = 2011
  - Month = May
- Ranked Top 3 products by revenue

### Task 7: Analytics
Performed analysis using SAP Web IDE:
- Total revenue for Germany in May 2011
- Top 3 products by generated revenue

## Learning Outcomes
Through this project, I gained hands-on experience in:

- SAP HANA XSA Development
- HDI Container Management
- Cross-container Access
- Data Modeling
- Calculation Views
- Star Schema Design
- Business Analytics using SAP HANA

## Author
Sharath Chandra Chandrashekhar

GitHub: https://github.com/SharathChandra-dev
