# Superstore Sales Dashboard | Power BI

<img width="1328" height="741" alt="Dashboard" src="https://github.com/user-attachments/assets/6b12357e-5938-46f3-bfd4-eb23028464e1" />


## Business Problem
A retail store manager wants to know:
1. How much did we sell, and how much profit did we make?
2. Which product categories make the most (and least) profit?
3. Which regions perform best?

## Dataset
Sample Superstore dataset (Kaggle): about 10,000 US retail sales records with category, sub-category, region, state, segment, sales, quantity, discount and profit.

## Tools
- Power BI Desktop
- Power Query (data type checks)
- DAX (measures)

## What I Built
- 4 KPI cards: Total Sales, Total Profit, Profit Margin %, Total Quantity
- Profit by Sub-Category (bar chart)
- Sales & Profit by Region (bar chart)
- Profit by State (map)
- Slicers for Ship Mode and Segment

## DAX Measures
```
Total Sales = SUM ( Superstore[Sales] )
Total Profit = SUM ( Superstore[Profit] )
Profit Margin % = DIVIDE ( [Total Profit], [Total Sales] )
Total Quantity = SUM ( Superstore[Quantity] )
```

## Key Insights
- Total sales of **$2.30M** with **$286K profit** (12.5% margin).
- **Technology** is the most profitable category (~$145K), led by Copiers, Phones and Accessories.
- **Tables, Bookcases and Supplies lose money**: Tables lost about $17.7K, Bookcases $3.5K and Supplies $1.2K.
- **West** leads with $725K sales and $108K profit (15% margin). **Central** sells $501K but makes only $40K profit (8% margin).

## Recommendations
- Review pricing and discounts on Tables and Bookcases, or reduce focus on them.
- Investigate why Central's margin is about half the West's.
- Promote high-margin Technology products more.

## Files
- `Superstore_Sales_Dashboard.pbix`: Power BI report
- `dashboard.png`: dashboard screenshot
