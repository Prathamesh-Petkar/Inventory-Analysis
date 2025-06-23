# Inventory Analysis

Inventory Dashboard Repository
Overview
This repository contains a Power BI dashboard designed to monitor and analyze inventory trends for two plants: Pears and TSP. The dashboard includes interactive visuals and DAX measures to provide insights into inventory levels, trends, and status.
Features

Slicers: 
Plant (Pears/TSP)
Items (all items across both plants)
Top N filter (5, 10, 15, 20, 25) for stacked bar chart (% increase per item)


Cards: 
Total inventory for both plants
Total warnings (items exceeding minimum past inventory)
Average % increase
Individual plant inventories (Pears and TSP)


Monthly Inventory Trend: Line graph with small multiples showing monthly inventory value trends for each item.
Plant Wise Inventory Trend: Line graph displaying monthly trends for both plants.
% Increase per Item: Stacked bar chart showing item-wise % increase compared to minimum past inventory.
Matrix Visual: Displays plants, their respective items, current inventory, minimum past inventory, and status.

Data

Source: Master file (Excel workbook with inventory data)
Columns: Plant, Items, Inventory_Value, Month_Order, Months
Data Points: Monthly inventory values from January 2025 to July 2025.

DAX Measures

Power Query: Month_Order for chronological sorting.
Base Measures: Latest_Month, Current_Month_Inventory.
Inventory Benchmarks: Min_Inventory_By_Item, Min_Past_Inventory_per_Item_per_Plant.
KPI Calculations: % Change, Inventory_Status.
Trend Analysis: Item Plant Trend Slope.
Aggregates and Totals: Avg_%_Increase, Total_Latest_Month_Inventory, Total_Min_Past_Inventory, Total_Warnings, Pears Current Inventory, TSP Current Inventory.
Top N Visuals: ItemRank, SelectedTopN, TopN_%Increase.

Usage

Clone the repository.
Open Closing inventory working.xlsx in Power BI.
Load the data and apply the provided DAX measures.
Explore the dashboard visuals and interact with slicers for detailed analysis.

Contributing
Feel free to fork this repository, submit issues, or propose enhancements via pull requests.
License
[Specify license, e.g., MIT] - Add appropriate license file if applicable.

