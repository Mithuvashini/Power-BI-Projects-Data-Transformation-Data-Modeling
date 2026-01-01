# Power BI – E-Commerce Sales Analysis

## Objective
Analyze e-commerce sales data using **Power BI** with a focus on **data transformation, modeling, and aggregation** to build analysis-ready datasets.

## Datasets Used
- **List of Orders.csv**
- **Order Details.csv**
- **Sales Target.csv**

---

## Data Import
- Imported all datasets into **Power BI**
- Used **Power Query Editor** for transformations

---

## Data Transformation
- Limited **List of Orders** to first **500 rows**
- Converted **Order Date** to `Date`
- Converted **Amount** and **Target** to `Fixed Decimal`
- Standardized **CustomerName** to Proper Case
- Created **Location** column (`City, State`)
- Created **Profit Margin (%)** = `Profit / Amount`
- Added **Profit Status**:
  - Loss → Profit < 0  
  - Break-Even → Profit = 0  
  - Profit → Profit > 0  

---

## Data Merging
- Merged **List of Orders** and **Order Details**
- Join Key: **Order ID**
- Final table: **Orders Data**

---

## Data Quality Handling
- Identified and handled:
  - Missing values (imputation/removal based on context)
  - Duplicate records (validated and removed where required)

---

## Sorting & Filtering
- Sorted orders by **Order Date (Descending)**
- Filtered data for **state-level analysis** (e.g., Tamil Nadu)

---

## Grouping & Aggregation
- **Order Details (Duplicate Table):**
  - Order count by Order ID
  - Average profit by Category
  - Total amount by Sub-Category
- **Sales Target (Duplicate Table):**
  - Total target aggregated by Month

---

## Data Modeling
- Relationship: **List of Orders ↔ Order Details**
  - Key: `Order ID`
- Relationship: **Order Details ↔ Sales Target**
  - Key: `Category`
- All relationships validated and active

---

## Tools Used
- Power BI
- Power Query
- Data Modeling & Aggregation Techniques

---

## Outcome
Delivered a **clean, structured, and analysis-ready data model** suitable for dashboarding and business insights.
