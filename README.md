# Sales Dashboard - Power BI Project

## Project Overview

### Title: Sales Dashboard

**Data Sources:**
- Microsoft Excel
- TXT CSV File

**Cleaning and Visualization Tools:**
- Power Query
- Power BI

## Understanding Data Sources:

### Microsoft Excel (Customer Master Dataset):

- **Customer ID:**
  - 663 unique customers
- **Customer Group**
- **Customer Name**
- **Customer Category Name**
- **Primary Contact**
- **Phone Number**
- **Fax Number**
- **Website URL**
- **Delivery Method**
- **City/Province:**
  - 49 provinces
  - Texas: 46 customers (highest)
  - Hawaii: 1 customer (lowest)

### TXT CSV File (Invoice Dataset):

- **InvoiceLineID**
- **CustomerCode**
- **TransactionID**
- **Description**
- **Year, Month, Day**
- **PackageTypeID**
- **Quantity**
- **Sales**
- **Total Dry Items**
- **Total Chiller Items**

## Cleaning and Visualization:

### Cleaning the Invoice Data:

1. Checked data types in Power Query.
2. Changed Sales column data type to Currency.
3. Merged Year, Month, and Day columns for a defined DATE column.
4. Converted the merged Date column data type from Text to Date.

### Cleaning the Customer Master Data:

1. Loaded the data into Power Query.
2. Used ETL method to transform the data.
3. Split CityProvince column into City and Province.
4. Removed unnecessary columns.
5. Loaded cleaned data into Power BI.

## Visualization:

1. **Establishing Relationships in the Data Model:**
   - Created a relationship between Invoice Data (CustomerCode) and Master Customer Data (CustomerID).

2. **Analysis:**
   - Analyzed Sales by Customer Category Name using a clustered Bar Chart.
   - Added a Year slicer for filtering.
   - Renamed "Sales by Customer Category Name" to "Sales by Category."
   - Introduced a table for Time Intelligence Analysis:
     - Sales value for each month.
     - Sales by month calculation.
     - Year over Year Percentage Change.
     - Sales by Year to Date.

3. **Visualizing Sales by Province:**
   - Used a Field map chart with Sales as KPI and Province from the Customer Master data.

4. **Visualizing Quantity by Month:**
   - Used a line chart with Quantity on the Y-axis and Month on the X-axis.

5. **KPI Card:**
   - Introduced a KPI card displaying the overall Quantity by year.

6. **Header:**
   - Added a Text box for the dashboard header.

## Power BI Dashboard Published Link:

[Sales Dashboard](https://app.powerbi.com/view?r=eyJrIjoiNWNmNDNmOWQtOTBlOC00ZTU1LWIxNjctMTk5MGVlNTA5OWM4IiwidCI6ImRmODY3OWNkLWE4MGUtNDVkOC05OWFjLWM4M2VkN2ZmOTVhMCJ9)

---
