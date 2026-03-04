# AtliQ-Hardware---Business-Insights-360

## 📊 AtliQ Hardwares – Cross-Functional BI & Profitability Analysis

### Project Overview

AtliQ Hardwares, a global computer and accessories company, was experiencing unexpected financial losses despite strong revenue growth in several regions. The company relied heavily on Excel-based reporting, limiting visibility across departments.

This project aimed to develop a unified Power BI reporting system integrating 1.8 million records from Excel, CSV, and MySQL into a single cross-functional analytics solution.

The objective was to empower stakeholders from Sales, Marketing, Finance, Supply Chain, and Executive leadership with centralized, drillable insights for smarter decision-making.

I worked on this project by following the Codebasics PowerBi Course,

Here is my report link - https://app.powerbi.com/view?r=eyJrIjoiMDhlYjhjYTctMWU3ZC00MzAyLWE0ZGUtNjQ2MDA2MzM3ODQ1IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9

### Dataset

The dataset used in this project contains 1.8M+ transactional records representing the operations of AtliQ Hardwares, a global electronics company operating in both Brick & Mortar and E-commerce channels.

Data was sourced from multiple systems to simulate a real-world enterprise data environment:
  - Excel files – Business planning data such as targets, budgets, and manual reports
  - CSV files – Sales transactions, product details, and customer information
  - MySQL database – Core operational data including orders, products, markets, and pricing information

The dataset captures multiple business domains including:
  - Sales transactions
  - Product hierarchy and categories
  - Customer and market segmentation
  - Pricing and discount structures
  - Financial performance metrics
  - Supply chain forecasting data

This multi-source dataset required extensive data cleaning, transformation, and standardization before being used for analytics.

### Data Modelling

To support cross-functional analytics, a snowflake schema data model was implemented consisting of 10+ interconnected tables.

The model was designed to enable scalable reporting across different business functions such as Finance, Sales, Marketing, Supply Chain, and Executive reporting.

#### Key Modelling Concepts

Dimension table: Static data like customer and product details.

Fact table: Transaction data.

gdb041:
  - dim_customer
  - dim_market
  - dim_product
  - fact_forecast_monthly - This table is used to forecast the customer’s need in advance, which can help in Higher customer satisfaction and reduced cost in
    warehouses for storage purposes
  - fact_sales_monthly - This table is more or less is same as the fact_forecast_monthly table, but the last column has the value of the sold quantity instead of      the forecast value.
    
gdb056:
  - freight_cost
  - gross_price
  - manufacturing_cost
  - Pre_invoice_dedutions
  - Post_invoice_deductions

The snowflake structure was used to normalize hierarchical data such as product categories and market segments, reducing redundancy while maintaining relational integrity.

<img width="720" height="792" alt="Data Model" src="https://github.com/user-attachments/assets/e2804a59-3ad6-4bd0-8723-ae5b796f26f0" />


Relationships were carefully designed to ensure:
  - Accurate aggregation across dimensions
  - Efficient filtering across dashboards
  - Consistent KPI calculations

A dedicated Measures Table was also implemented to organize DAX measures and maintain a clean semantic layer.

<img width="392" height="690" alt="Key Measures" src="https://github.com/user-attachments/assets/a81fc2f9-cedd-4a56-a5c5-c37880fcbc37" />


### Technical Highlights
  - Built a snowflake schema data model with 10+ tables
  - Cleaned and transformed data using advanced Power Query operations
  - Created basic and complex DAX measures for cross-functional KPIs
  - Designed user-empathetic, stakeholder-focused dashboards
  - Implemented drill-through functionality for root cause analysis
  - Used bookmarks for seamless navigation
  - Deployed the solution in Power BI Service
  - Iteratively refined the dashboard based on stakeholder feedback

    
### Key Business Insight

While analyzing regional performance, the dashboard revealed:
  - Certain regions showed strong revenue growth
  - However, profitability remained significantly lower
  - Drill-down analysis identified excessive discounting as the primary driver of margin erosion
    
This insight highlighted that revenue growth was being achieved at the cost of profitability, enabling leadership to reconsider pricing and discount strategies.


### Dashboard Structure

Home – Central navigation

<img width="1302" height="732" alt="Home" src="https://github.com/user-attachments/assets/243abe9a-4cc6-4b92-96e3-d7660e23aec0" />

------------------------------------------------------------------------------------------------------------------------------------------------------------------
Finance – Profitability & margin analysis

<img width="1306" height="731" alt="Finance" src="https://github.com/user-attachments/assets/ff856bd5-f66a-4d78-80db-5b41a3b15336" />

------------------------------------------------------------------------------------------------------------------------------------------------------------------
Sales – Revenue trends & regional performance

<img width="1306" height="731" alt="Sales" src="https://github.com/user-attachments/assets/40e1a4f9-a4a7-42a0-9c65-b734a51ac956" />

------------------------------------------------------------------------------------------------------------------------------------------------------------------
Marketing – Campaign effectiveness

<img width="1302" height="732" alt="Marketing" src="https://github.com/user-attachments/assets/dbc3ebed-66cf-4002-a446-9ccf4fb45f8f" />

------------------------------------------------------------------------------------------------------------------------------------------------------------------
Supply Chain – Inventory & operational metrics

<img width="1305" height="732" alt="Supply Chain" src="https://github.com/user-attachments/assets/51cf1c39-6160-4880-8767-0d40911a89cc" />

------------------------------------------------------------------------------------------------------------------------------------------------------------------
Executive – High-level KPI overview

<img width="1300" height="732" alt="Executive" src="https://github.com/user-attachments/assets/5a0376f2-2fd5-4182-aa37-2f415aa961cb" />

------------------------------------------------------------------------------------------------------------------------------------------------------------------
### Outcome

The final model enabled the creation of a unified analytics platform where stakeholders can explore insights through interactive dashboards covering Finance, Sales, Marketing, Supply Chain, and Executive views.


