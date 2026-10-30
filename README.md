# Week 01 – Data Understanding

## Objective

Understand the Heavy Suppliers & Warehouse dataset, its business context, table structure, columns, and relationships.

## Work Completed

* Reviewed all 12 datasets and their schemas.
* Identified dimensions, transaction tables, and master data.
* Examined row counts, data types, null values, and duplicate records.
* Identified primary and foreign-key candidates.
* Documented important business entities such as customers, suppliers, products, branches, sales, purchases, invoices, payments, and stock movements.

## Tools Used

* Power BI
* Power Query
* Excel
* CSV datasets

## Outputs

* Dataset inventory
* Data dictionary
* Initial data-quality observations
* Identified fact and dimension tables

## Key Insights

* The project contains 12 interconnected datasets covering sales, purchasing, suppliers, inventory, warehouses, invoices, payments, and stock movements.
* Several tables require validation before being used as relationship keys.
* Transaction tables contain significantly more records than master tables, making a star-schema model appropriate.

  ----------------------------------
# Week 02 – Data Cleaning & Transformation

## Objective

Prepare the raw datasets for reliable analysis by correcting data types, cleaning text, and validating data quality.

## Work Completed

* Removed blank rows and unnecessary spaces.
* Applied Trim and Clean transformations to text columns.
* Standardized date, numeric, and text data types.
* Converted warehouse capacity values into numeric values.
* Handled null values appropriately.
* Created validation columns for stock and transaction data.
* Checked duplicate IDs and inconsistent records.

## Tools Used

* Power Query
* Power BI
* Excel

## Outputs

* Cleaned datasets
* Data-quality validation
* Standardized columns
* Transformation queries

## Key Insights

* Some IDs contain duplicates and require business-level validation before creating one-to-many relationships.
* Cancelled purchase orders contain blank received dates, which should be preserved rather than replaced.
* Inventory stock values require additional validation against stock ledger movements.

  ---------------------
  # Week 03 – Data Modeling

## Objective
Build a scalable Power BI data model connecting master, transaction, and date tables.

## Work Completed
- Created dimension tables for Branch, Customer, Product, Supplier, and Date.
- Organized transactional data into fact tables.
- Created one-to-many relationships.
- Applied single-direction cross-filtering.
- Connected sales and purchase headers with their respective line tables.
- Created active and inactive date relationships.
- Developed the `DimDate` table using DAX.

## Tools Used
- Power BI
- Power Query
- DAX

## Outputs
- Star-schema data model
- Relationship diagram
- DimDate table
- Active/inactive date relationships

## Key Insights
- A star schema provides cleaner filtering and easier DAX calculations.
- Header-to-line relationships support detailed transaction analysis.
- Inactive date relationships allow analysis using delivery, expected delivery, received, and due dates.

  ## Screenshots of One to Many Relationships
  <img width="1290" height="611" alt="Screenshot 2026-10-06 123900" src="https://github.com/user-attachments/assets/0983853d-db88-4037-b829-36304f926b4a" />
  <img width="1322" height="624" alt="Screenshot 2026-10-06 123927" src="https://github.com/user-attachments/assets/b764812b-94fb-4e54-8f58-7cd26f79f69d" />
  <img width="1298" height="627" alt="Screenshot 2026-10-06 123952" src="https://github.com/user-attachments/assets/f66e51cc-0614-456e-bcf0-892e524daff5" />
  <img width="1363" height="660" alt="Screenshot 2026-10-06 124027" src="https://github.com/user-attachments/assets/9c02e5e7-b290-4762-b50a-1e46ffbd0d2c" />
----------------------
# Week 04 – Sales Analysis

## Objective
Analyze sales performance across customers, products, branches, channels, and time.

## Work Completed
- Analyzed sales orders and sales order lines.
- Created sales KPIs and measures.
- Analyzed sales by product, category, branch, customer, and sales channel.
- Examined order trends over time.
- Analyzed delivery performance.
- Added interactive date and business filters.

## Tools Used
- Power BI
- DAX
- Power Query

## Outputs
- Sales analysis dashboard
- KPI cards
- Sales trend visuals
- Product and branch analysis

## Key Insights
- Sales performance can be analyzed at both order and line-item level.
- Time-based analysis helps identify changes in sales demand.
- Branch, product, and sales-channel analysis provides a detailed view of business performance.
-------------------------------------
# Week 05 – Purchase Order Analysis

## Objective
Analyze purchasing activity, purchase costs, delivery performance, and order status.

## Work Completed
- Analyzed purchase order headers and line items.
- Calculated purchase value and GST-related metrics.
- Analyzed purchase orders by supplier and branch.
- Compared expected and actual delivery dates.
- Analyzed purchase order status.
- Created supplier and purchase performance visuals.

## Tools Used
- Power BI
- DAX
- Power Query

## Outputs
- Purchase analysis dashboard
- Purchase KPIs
- Supplier purchase analysis
- Delivery performance analysis

## Key Insights
- Purchase analysis helps monitor procurement volume and supplier activity.
- Expected versus received dates can be used to evaluate delivery performance.
- Supplier and branch-level analysis supports procurement monitoring.
--------------------------------
# Week 06 – Supplier Analysis

## Objective
Evaluate supplier performance based on reliability, lead time, purchase activity, and regional information.

## Work Completed
- Analyzed supplier master data.
- Compared suppliers by region and product category.
- Examined supplier lead times.
- Analyzed reliability scores.
- Connected suppliers with purchase orders.
- Created supplier performance KPIs.

## Tools Used
- Power BI
- DAX
- Power Query

## Outputs
- Supplier analysis dashboard
- Supplier KPI cards
- Supplier comparison visuals
- Lead-time analysis

## Key Insights
- Supplier performance can be evaluated using multiple operational indicators rather than purchase value alone.
- Lead time and reliability are important dimensions for procurement analysis.
- Regional supplier analysis helps understand the supplier network.
--------------------
# Week 07 – Inventory Analysis

## Objective
Analyze inventory levels and identify products requiring stock monitoring.

## Work Completed
- Analyzed inventory by product and branch.
- Compared current stock with reorder, safety, and maximum stock levels.
- Created stock-status validation logic.
- Identified potential reorder and overstock conditions.
- Connected inventory with product and branch dimensions.

## Tools Used
- Power BI
- DAX
- Power Query

## Outputs
- Inventory dashboard
- Stock-status indicators
- Product stock analysis
- Branch inventory analysis

## Key Insights
- Inventory levels should be evaluated against reorder, safety, and maximum-stock thresholds.
- Product-level analysis helps identify items requiring further investigation.
- Current stock values should be validated against stock movement records before making operational decisions.
  




