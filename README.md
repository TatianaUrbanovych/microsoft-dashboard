# Microsoft Financial Analysis Dashboard - Power BI

## Project Overview
This project is an interactive Power BI dashboard designed to analyze and visualize the financial performance of Microsoft. It provides deep insights into the company's income statements, balance sheets, and overall financial health over a multi-year period (2016–2023, with projections up to 2026).

## Dashboard Features
The report is divided into key analytical sections:

### 1. Financial Performance & Profitability
* **Revenue vs. Cost:** An area chart tracking total revenue against total costs over time.
* **Operating Income vs. Expense:** A visual comparison of operational profitability.
* **Net Profit Tracking:** A detailed matrix and KPI gauge comparing actual net profit against target goals.
* **Future Projections:** A line chart featuring a forecast band for projected net profit up to 2026.

<img width="1333" height="742" alt="image" src="https://github.com/user-attachments/assets/9ea33d2b-3448-4fa6-834b-3e297b8824bc" />


### 2. Balance Sheet & Liquidity Analysis
* **Liquidity Ratios:** Dynamic card visuals calculating Current Ratio, Quick Ratio, and Absolute Liquidity.
* **Assets Breakdown:** A detailed pie chart categorizing short-term and long-term assets.
* **Liabilities Breakdown:** A visual distribution of liabilities, including long-term debt and common stock.
* **Interactive Filtering:** Slicers allowing users to filter balance sheet metrics by specific years.

<img width="1322" height="750" alt="image" src="https://github.com/user-attachments/assets/aa2a0622-68aa-4bc8-93d0-185352edd1d1" />


## Data Model & Schema
The project utilizes a structured relational data model (Star/Snowflake schema) to ensure accurate calculations and efficient filtering:
* **Fact Tables:** `Income Statement`, `Assets Info`, `Liabilities Info`.
* **Dimension Tables:** `Assets List`, `Liabilities List`.
* **Date Table:** A central `Calendar` table linked to all fact tables to enable time-intelligence DAX functions.

<img width="1473" height="742" alt="image" src="https://github.com/user-attachments/assets/62880eb5-b948-4ceb-bf67-fcda6f9f9cf4" />


## Key DAX Measures
Several custom DAX measures were created to drive the insights, including:
* **Profitability Metrics:** `Net Profit`, `Operating Income`, `Gross Income`, `Profitability %`.
* **Liquidity Ratios:** `Current liquidity ratio`, `Quick ratio`, `Absolute liquidity ratio`.
* **Time Intelligence:** `Net profit, previous year`.
* **Target Tracking:** `Target income`.

## Tools Used
* **Power BI Desktop:** Data modeling, DAX calculations, and visualization.
* **Power Query:** Data cleaning and transformation.

## How to Use
1. Download the `Microsoft.pbix` file from this repository.
2. Open the file using **Power BI Desktop**.
3. Use the slicers on the left panel or the year buttons to interact with the data and explore specific financial periods.

---
*Note: This is a portfolio project. Data is based on historical public financial statements.*
