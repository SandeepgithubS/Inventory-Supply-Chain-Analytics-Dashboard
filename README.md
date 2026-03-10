# Inventory & Supply Chain Analytics Dashboard

**Interactive real-time dashboard for inventory monitoring, supply chain visibility, and operational decision-making**  
Built with **Python**, **Streamlit**, and **MySQL**

## Project Overview

This project delivers a modern, user-friendly **Inventory & Supply Chain Analytics Dashboard** that enables businesses to:

- Track live inventory KPIs
- Monitor supplier and product status
- Manage sales, restocking, and reorder workflows
- Maintain full audit trail of stock movements

The application demonstrates end-to-end skills in **data engineering**, **database design**, **business logic implementation**, and **interactive analytics UI development**.

## Key Features

- Real-time **inventory KPIs**  
  – Total suppliers, products & categories  
  – 3-month rolling sale & restock value  
  – Products below reorder level (urgent attention flag)

- **Product lifecycle operations**  
  – Add new products (via stored procedure with manual ID control)  
  – View complete inventory history per product  
  – Place reorders  
  – Mark reorders as received (stored procedure)

- Clean separation of concerns  
  – Modular database layer (`db_function.py`)  
  – Secure form validation & error handling  
  – Responsive Streamlit interface with sidebar navigation & metric cards

## Tech Stack

| Layer                  | Technology                            |
|------------------------|---------------------------------------|
| Frontend / UI          | Streamlit                             |
| Backend / Data Layer   | Python · MySQL Connector              |
| Database               | MySQL (with stored procedures)        |
| Data Manipulation      | pandas                                |
| Layout & Components    | Streamlit columns, metrics, forms     |

## Main Dashboard Sections

### 1. Basic Metrics Overview
High-level KPIs at a glance:
- Total Suppliers
- Total Products
- Distinct Categories
- Sales Value (last 3 months)
- Restock Value (last 3 months)
- Products below reorder level (no pending reorder)

### 2. Supplier & Product Tables
- Supplier contact details
- Products with current stock, reorder level & assigned supplier
- Quick visibility into stock health and supplier dependencies

### 3. Product Inventory History
- Select any product → view chronological stock changes
- Tracks sales, restocks, and manual adjustments over time

### 4. Reorder Management Workflow
- Place new reorder requests
- View all pending/ordered reorders
- Mark orders as received → instantly updates inventory

## Business Value Demonstrated

- Provides **actionable visibility** into inventory risk (low stock alerts)
- Automates **routine supply chain tasks** (reorder placement & receipt)
- Maintains **data integrity** through stored procedures
- Enables **audit-ready traceability** of every stock movement
- Bridges **operational execution** and **analytics monitoring** in one tool
