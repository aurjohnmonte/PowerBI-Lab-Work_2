# 📊 Laboratory Work 2  
## End-to-End Data Analytics in Power BI: From Data Cleaning to DAX Insights

---

## 📑 Table of Contents
1. [Power Query – Data Cleaning](#power-query--data-cleaning)
2. [Open Power Query Editor](#open-power-query-editor)
3. [Remove Duplicates](#remove-duplicates)
4. [Handle Missing Values](#handle-missing-values)
5. [Change Data Types](#change-data-types)
6. [Rename Columns Properly](#rename-columns-properly)
7. [Applied Steps Screenshot](#applied-steps-screenshot)
8. [Guide Questions](#guide-questions)
9. [Enhancement Activities](#enhancement-activities)
10. [Merge and Append Queries](#merge-and-append-queries)
11. [Merge Datasets](#merge-datasets-inner-join)
12. [Append Queries](#append-queries)
13. [Validate Data](#validate-merged-data)

---

# Power Query – Data Cleaning

## 🎯 Lab Objectives

- Clean and prepare raw datasets
- Apply data transformation techniques in **Power Query**

---

# Open Power Query Editor

### Steps

1. Open **Power BI Desktop**
2. Click **Home → Get Data → Excel Workbook**
3. Select **Messy_Sales_Data.xlsx**
4. Click **Transform Data** to open **Power Query Editor**

### Screenshot

<img src="images/open-power-query.png" width="800">

### Explanation

The **Power Query Editor** allows users to clean, transform, and prepare raw datasets before they are loaded into Power BI for analysis. It is an essential step in the data preparation process.

---

# Remove Duplicates

### Steps

1. Select the dataset table.
2. Highlight the **OrderID** column.
3. Click **Home → Remove Rows → Remove Duplicates**.

### Screenshot

<img src="images/remove-duplicates.png" width="800">

### Explanation

Removing duplicates ensures that every **OrderID** represents a unique transaction. Duplicate data can lead to incorrect calculations, inaccurate reports, and misleading business insights.

---

# Handle Missing Values

### Methods Used

| Method | Description |
|------|------|
| Replace Values | Replace null values with `0` |
| Remove Blank Rows | Remove rows with missing data |
| Fill Down | Copy previous value downward |

### Steps

1. Identify columns containing **null values**
2. Apply appropriate transformation:
   - **Transform → Replace Values**
   - **Remove Rows → Remove Blank Rows**
   - **Transform → Fill → Down**

### Screenshot

<img src="images/missing-values.png" width="800">

### Explanation

Missing values can cause issues in reports and analytics. Handling them properly ensures the dataset remains accurate and usable.

---

# Change Data Types

### Correct Data Types

| Column | Data Type |
|------|------|
| Order Date | Date |
| Sales | Decimal Number |
| Quantity | Whole Number |

### Steps

1. Check the **data type icon** beside each column name.
2. Change to the appropriate type if necessary.

### Screenshot

<img src="images/change-data-types.png" width="800">

### Explanation

Correct data types ensure Power BI performs calculations accurately and allows features such as time analysis and numeric aggregation.

---

# Rename Columns Properly

### Naming Convention

| Original Name | New Name |
|------|------|
| Order ID | `order_id` |
| Order Date | `order_date` |
| Customer Name | `customer_name` |
| Sales | `total_sales` |

### Screenshot

<img src="images/rename-columns.png" width="800">

### Explanation

Using consistent naming conventions improves readability and makes it easier to write **DAX formulas, queries, and reports**.

---

# Applied Steps Screenshot

<img src="images/applied-steps.png" width="800">

### Explanation

The **Applied Steps pane** records every transformation applied in Power Query. This allows analysts to review, modify, and reproduce the data cleaning process.

---

# Guide Questions

## 1. Why is removing duplicates important in data analysis?

Removing duplicates ensures that each record represents a unique transaction. Duplicate data can inflate totals, distort analytics, and lead to incorrect conclusions in reports.

---

## 2. What problems can missing values cause in reports?

Missing values may cause:

- Incorrect calculations
- Broken visualizations
- Misleading insights
- Errors in data aggregation

Handling missing values ensures reliable reporting.

---

## 3. How does correct data typing affect calculations?

Correct data types ensure Power BI performs appropriate operations. For example:

- **Date types** allow time-based analysis
- **Decimal numbers** support financial calculations
- **Whole numbers** support counting and aggregation

Incorrect data types may lead to errors or invalid calculations.

---

## 4. What naming conventions improve data readability?

Good naming conventions include:

- Use lowercase letters
- Use underscores instead of spaces
- Use descriptive column names

Example:
