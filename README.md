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

