# Analyze Data in a Model Car Database with MySQL Workbench

This project is part of my Coursera coursework where I analyze data from Mint Classics, a classic model car retailer, to support business decisions on inventory management and warehouse consolidation.

## Project Overview
Mint Classics is planning to close one of its storage facilities. Using SQL in MySQL Workbench, I explored the company’s inventory and sales data to provide data-driven recommendations that improve efficiency and reduce costs.

---

## Project Objectives
1. Explore current inventory products.
2. Identify key factors affecting inventory reorganization.
3. Provide analytical insights and actionable recommendations.

---

## Approach & Tasks

### Task 1 – Import Database  
Imported the `mintclassicsDB.sql` script into MySQL Workbench to create the relational database with nine tables containing warehouse, product, sales, and inventory data.

![Import database screenshot](https://github.com/thienhuongdn2002/Analyze-Data-in-a-Model-Car-Database-with-MySQL-Workbench/blob/main/Picture1.png)

---

### Task 2 – Understand the Data & Business Process  
- Identified 4 warehouses with varying capacities.

![Warehouses and capacities](https://github.com/thienhuongdn2002/Analyze-Data-in-a-Model-Car-Database-with-MySQL-Workbench/assets/144947062/8a3f07be-6bd9-4b54-a720-69b968a714fd)

- Counted 110 unique products in inventory.
- Found no product overlap between warehouses.
- Analyzed product lines per warehouse and their stock levels.

![Products per warehouse and stock](https://github.com/thienhuongdn2002/Analyze-Data-in-a-Model-Car-Database-with-MySQL-Workbench/assets/144947062/da317085-f42e-4ccf-8706-4aaeb0ef60bd)

- Identified product lines stored in each warehouse.

![Product lines by warehouse](https://github.com/thienhuongdn2002/Analyze-Data-in-a-Model-Car-Database-with-MySQL-Workbench/assets/144947062/a8b4dd7d-c174-490c-bdc9-50f6f99ee6ed)

- Determined product lines with highest and lowest sales.

![Sales by product line](https://github.com/thienhuongdn2002/Analyze-Data-in-a-Model-Car-Database-with-MySQL-Workbench/assets/144947062/9e7a5aa9-4153-4265-98d8-a638eb352c03)

---

### Task 3 – Business Issue Investigation  
Created a temporary table to compare stock against orders to classify products as overstocked, well-stocked, or understocked by warehouse.

![Temporary table for inventory status](https://github.com/thienhuongdn2002/Analyze-Data-in-a-Model-Car-Database-with-MySQL-Workbench/assets/144947062/818f2029-45dc-43d4-9b40-980dd44d9476)

Identified overstock quantities per warehouse:

![Overstock by warehouse](https://github.com/thienhuongdn2002/Analyze-Data-in-a-Model-Car-Database-with-MySQL-Workbench/assets/144947062/324eb642-670e-4641-87fe-18c1f1117f65)

![More overstock data](https://github.com/thienhuongdn2002/Analyze-Data-in-a-Model-Car-Database-with-MySQL-Workbench/assets/144947062/292ea044-697b-4f65-8f9c-8134f6a27eed)

Warehouse B had the highest overstocked products (29), while Warehouses A and C each had 19 overstocked items.

Analyzed sales percentages and inventory for each product line:

![Product line sales and inventory](https://github.com/thienhuongdn2002/Analyze-Data-in-a-Model-Car-Database-with-MySQL-Workbench/assets/144947062/e3334e33-c601-46d5-b65f-42699a57995a)

---

### Task 4 – Warehouse Consolidation Recommendation  

- Warehouse B holds Classic Cars, has the highest capacity, but suffers from overstock and lower sales.  
- Warehouse C has the lowest utilization (50%) and storage capacity, indicating wasted space.  

**Recommendation:** Close Warehouse C and relocate its inventory to Warehouse B.

**Benefits:**  
- Optimized space usage leveraging Warehouse B's capacity.  
- Streamlined inventory management with fewer locations.  
- Cost savings on operational expenses.

---

## Summary

This project showcases my SQL expertise and ability to use data-driven insights to optimize inventory and warehouse management strategies.

---

Feel free to explore the repository for queries, analysis scripts, and detailed findings.
