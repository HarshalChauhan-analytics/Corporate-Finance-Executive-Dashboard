# Corporate Finance Executive Dashboard 📊

## Project Overview
This project is an end-to-end business intelligence solution designed to track corporate sales performance, profitability, and geographic revenue trends. Built in **Power BI**, the dashboard provides executives with a high-contrast, interactive interface to analyze critical financial KPIs over time and across multiple product segments.

### 🖼️ Dashboard Preview
*(Drag and drop your JPG screenshot right here! Delete this text once the image uploads)*

## Technical Skills Demonstrated
* **Data Extraction & Transformation (ETL):** Utilized **Power Query** to clean raw financial data, standardize text formatting, and prepare the dataset for analysis.
* **Data Modeling:** Built a robust relational data model, including a custom-generated Calendar table to enable complex time-intelligence tracking.
* **Advanced DAX (Data Analysis Expressions):** Programmed custom measures to calculate dynamic business logic, bypassing standard drag-and-drop aggregations.
* **Visual Hierarchy & Theming:** Designed an "Executive Wide" layout utilizing a custom-coded JSON "Neon Tech Dark Mode" theme for optimized scannability and contrast.

## Key Performance Indicators (KPIs) Calculated
The following metrics were built using custom DAX formulas:
* **Total Revenue:** `SUM(financials[Sales])`
* **Gross Profit Margin %:** `DIVIDE(SUM(financials[Profit]), [Total Revenue], 0)`
* **Year-to-Date (YTD) Revenue:** `TOTALYTD([Total Revenue], 'Calendar'[Date])`

## Insights & Interactivity
* **Dynamic Slicing:** Users can filter the entire report by specific countries or timeframes using the dropdown slicer.
* **Trend Analysis:** A wide-screen line chart maps revenue spikes and dips across the fiscal year.
* **Profitability Breakdown:** A matrix table and donut chart reveal exactly which market segments (e.g., Government, Enterprise, Small Business) are driving the most value.
