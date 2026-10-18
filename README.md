# 📊 Power BI Semantic Model Design & Data Modeling (PL-300 Lab 03)

## 📌 Project Overview
This repository contains the data model design for the **AdventureWorks** dataset as part of the **Microsoft PL-300: Power BI Data Analyst** certification coursework. 

The primary objective of this laboratory was to transform raw tables into a highly optimized **Star Schema** (Data Model), establishing relationships, defining cardinality, setting cross-filtering directions, and preparing the semantic model for advanced DAX analytics.

---

## 🛠️ Key Tasks & Technical Implementation

1. **Star Schema Architecture:**
   - Identified and structured the central **Fact Table** (`Sales`) containing transactional metrics and numeric key attributes.
   - Connected Dimension Tables (**`Product`**, **`Reseller`**, **`Region`**, **`Salesperson`**, **`SalespersonRegion`**, **`Targets`**) to provide descriptive attributes for filtering and slicing.

2. **Relationship Configuration & Cardinality:**
   - Established **One-to-Many (`1:*`)** relationships between dimension primary keys ($PK$) and fact foreign keys ($FK$).
   - Configured cross-filter direction to **Single** (flowing from Dimensions to Facts) to maintain high performance and avoid circular dependency.

3. **Data Model Optimization & Usability:**
   - **Hidden Foreign Keys:** Omitted technical foreign key columns from the Report View to prevent incorrect aggregation and improve end-user experience.
   - **Date Table Configuration:** Configured the date dimension using **Mark as Date Table** to enable time-intelligence function capabilities in DAX.
   - Categorized data types and field formatting (e.g., Currency, Percentages, and Spatial Data Types).

---

Project completed as part of the PL-300 Data Analyst Learning Path.
