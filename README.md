# DBR361 Assignment 2 – AdventureWorks Business Intelligence Report

## Project Overview

This project was completed for **DBR361** and focuses on designing and developing a **SQL Server Reporting Services (SSRS)** business intelligence report using the **AdventureWorks2022** database.

The report integrates multiple datasets, report parameters, visualizations, and performance indicators to provide actionable insights into:

- Product sales performance
- Salesperson effectiveness
- Territory-based sales analysis
- Customer shipping and tax costs
- Product category trends

The solution was developed using **SQL Server**, **SSRS (.rdl)**, and the **AdventureWorks2022** sample database.

---

## Repository Structure

```text
DBR361_Assignment_2_Group_O/
│
├── DBR361_Assignment_2-Group_O.final..rdl
├── DBR361_Assignment_2-Group_O.final..pdf
└── README.md
```

---

## Technologies Used

- Microsoft SQL Server
- SQL Server Reporting Services (SSRS)
- AdventureWorks2022 Database
- T-SQL
- Report Builder / Power BI Report Builder

---

## Report Features

### 1. Product Information by Category

Displays detailed product information including:

- Product ID
- Product Name
- Product Subcategory
- Product Category
- Order Quantity
- Sales Revenue (Line Total)

#### Parameter
- **ProdName** (Multi-select parameter)

Users can select one or multiple products to analyze their sales performance.

---

### 2. Product Sales Analysis by Category

Provides category-level sales insights by combining:

- Product Categories
- Product Subcategories
- Order Quantities
- Unit Prices
- Sales Orders
- Order Years

#### Key Metrics

- Total Sales Revenue
- Sales Quantity
- Product Category Performance
- Yearly Sales Trends

---

### 3. Salesperson Performance Dashboard

Analyzes sales performance across territories and stores.

#### Included Information

- Salesperson ID
- Salesperson Name
- Territory
- Store Name
- Sales Quota
- Order Quantity
- Revenue Generated

#### Parameter

- **Territory**

Users can filter results by sales territory.

#### Performance Indicator

The report includes indicators comparing:

- Actual Sales
- Sales Quotas

This enables quick identification of high-performing and under-performing sales representatives.

---

### 4. Territory and Store Analysis

Provides relationships between:

- Stores
- Salespersons
- Sales Territories

This section helps evaluate territory coverage and sales distribution.

---

### 5. Customer Freight and Tax Analysis

Analyzes customer-related expenses using:

- Freight Costs
- Tax Amounts
- Customer Information
- Sales Orders

#### Metrics Included

- Total Freight Expenses
- Total Tax Obligations
- Customer-Level Cost Analysis

---

## Database

### Data Source

**AdventureWorks2022**

The report connects to SQL Server using an integrated security connection and retrieves data from:

- Production.Product
- Production.ProductCategory
- Production.ProductSubcategory
- Sales.SalesOrderHeader
- Sales.SalesOrderDetail
- Sales.Customer
- Sales.Store
- Sales.SalesPerson
- Sales.SalesTerritory
- Person.Person
- Sales.SalesPersonQuotaHistory

---

## Key Business Questions Answered

### Product Analysis

- Which products generate the highest sales revenue?
- Which product categories perform best?
- How do sales vary across categories?

### Salesperson Analysis

- Which salespeople exceed their quotas?
- Which territories generate the most revenue?
- How does salesperson performance compare across stores?

### Customer Analysis

- Which customers incur the highest freight costs?
- What are the overall tax obligations associated with orders?

### Territory Analysis

- Which territories contribute most to total sales?
- How are stores distributed across territories?

---

## Learning Outcomes

This project demonstrates practical skills in:

- Database querying with T-SQL
- Data modeling and joins
- SSRS report development
- Parameterized reporting
- KPI and indicator implementation
- Business intelligence reporting
- Data visualization and decision support

---

## How to Run

### Prerequisites

- SQL Server
- AdventureWorks2022 Database
- SQL Server Reporting Services (SSRS)
- Power BI Report Builder or Report Builder

### Steps

1. Restore the AdventureWorks2022 database.
2. Open the `.rdl` file in Report Builder.
3. Update the data source connection if necessary.
4. Run the report.
5. Use the report parameters to filter and analyze data.

---

## Report Parameters

| Parameter | Type | Purpose |
|------------|------|----------|
| ProdName | Multi-select | Filter products for analysis |
| Territory | Single-select | Filter salesperson performance by territory |

---

## Project Information

**Author:** Alisa Peacock
**Module:** DBR361  
**Project Type:** Business Intelligence & Reporting  
**Database:** AdventureWorks2022  
**Platform:** SQL Server Reporting Services (SSRS)

---

