<img width="1641" height="646" alt="image" src="https://github.com/user-attachments/assets/2fa2e6f6-da68-48e1-9be7-a22b0cfa151d" />


# iPhone Sales Interactive Dashboard

An interactive sales analytics dashboard built in Microsoft Excel, powered by the `iphone_sales_dataset.csv` dataset. It delivers real-time insights into iPhone sales performance across models, countries, time periods, and payment methods using PivotTables, PivotCharts, Slicers, and a Timeline.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Features](#features)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Building the Dashboard](#building-the-dashboard)
- [KPIs](#kpis)
- [Interactivity](#interactivity)
- [Maintenance](#maintenance)
- [Requirements](#requirements)

## Overview

This project transforms raw iPhone sales records into a fully interactive Excel dashboard. Users can filter the entire view by country, model, storage, color, payment method, and date range, with all charts and KPI cards updating simultaneously.

## Dataset

Source file: `iphone_sales_dataset.csv`

| Column | Description | Example |
| --- | --- | --- |
| `Order_ID` | Unique identifier for each order | `1001` |
| `Customer_Name` | Name of the customer | `Customer_1` |
| `Country` | Country where the sale occurred | `USA` |
| `iPhone_Model` | iPhone model sold | `iPhone 15 Pro Max` |
| `Storage` | Storage capacity | `256GB` |
| `Color` | Device color | `Purple` |
| `Quantity` | Number of units sold | `5` |
| `Price` | Unit price | `1817` |
| `Sale_Date` | Date of sale (YYYY-MM-DD) | `2025-05-01` |
| `Payment_Method` | Payment method used | `Debit Card` |

### Sample Records

| Order_ID | Customer_Name | Country | iPhone_Model | Storage | Color | Quantity | Price | Sale_Date | Payment_Method |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1001 | Customer_1 | USA | iPhone 13 | 256GB | Purple | 5 | 1817 | 2025-05-01 | Debit Card |
| 1002 | Customer_2 | Canada | iPhone 12 | 256GB | Blue | 1 | 998 | 2025-03-05 | PayPal |
| 1003 | Customer_3 | Canada | iPhone 15 Pro Max | 512GB | Black | 5 | 876 | 2025-01-25 | Credit Card |
| 1004 | Customer_4 | USA | iPhone 15 Pro Max | 512GB | Black | 2 | 1290 | 2025-03-24 | Debit Card |
| 1005 | Customer_5 | USA | iPhone 15 | 128GB | Blue | 3 | 1092 | 2025-02-01 | Debit Card |

## Features

- Revenue analysis by iPhone model, country, and month
- Sales volume breakdown by payment method
- KPI cards for high-level metrics (Total Revenue, Total Units)
- Cross-filtering with Slicers and a date Timeline
- One-click refresh when the source data changes

## Project Structure

iphone-sales-dashboard/

├── iphone_sales_dataset.csv # Raw source data

├── Dashboard.xlsx # Excel workbook with the dashboard

│ ├── SalesData (sheet) # Imported table + Revenue column

│ ├── Pivots (sheet, hidden) # PivotTables powering the charts

│ └── Dashboard (sheet) # Final visual dashboard

└── README.md
