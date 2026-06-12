# Customer Segmentation Dashboard (Power BI)

## Overview
This project segments customers based on their demographic and behavioral
data using Microsoft Power BI. The dashboard groups customers into five
distinct segments and visualizes their purchasing patterns, spending habits,
and preferences to support targeted marketing decisions.

## Dataset
The dataset (`customer_data.xlsx`) contains 500 customer records with the
following fields:

- **CustomerID** – Unique identifier for each customer
- **Age** – Customer's age
- **Gender** – Male / Female
- **AnnualIncome_k** – Annual income (in thousands)
- **SpendingScore** – Score (0–100) reflecting spending behavior
- **PurchaseFrequency_per_month** – Average purchases per month
- **AvgOrderValue** – Average value per order
- **PreferredCategory** – Most frequently purchased product category

## Methodology
- Customer segments were created using a calculated DAX column based on
  income, spending score, age, and purchase frequency.
- Five segments were identified:
  1. **High-Income Frequent Spenders** – highest income, highest spending, frequent buyers
  2. **Occasional Premium Buyers** – high income, low frequency, very high order value
  3. **Frequent Bargain Hunters** – moderate income, highest purchase frequency
  4. **Average Middle-Class Shoppers** – balanced metrics across the board
  5. **Young Budget Shoppers** – youngest, lowest income and spending

## Dashboard Features
- **KPI Cards**: Total Customers, Average Spending Score, Average Order Value
- **Bar Chart**: Number of customers per segment
- **Scatter Chart**: Annual Income vs Spending Score, colored by segment
- **Scatter Chart**: Purchase Frequency vs Average Order Value, colored by segment
- **Stacked Bar Chart**: Preferred category breakdown by segment
- **Summary Table**: Average Age, Income, Spending Score, Order Value, and
  Purchase Frequency per segment
- **Slicers**: Filter by Segment, Preferred Category, and Gender

## Key Insights
- High-Income Frequent Spenders generate the highest average order value
  (~4,032) and spending score (~78) — ideal targets for premium offers and
  loyalty programs.
- Occasional Premium Buyers have high income but low purchase frequency,
  with very high order values — suited for seasonal or big-ticket promotions.
- Frequent Bargain Hunters shop most often (~11.4 times/month) but at lower
  order values — respond well to discounts and bundle deals.
- Young Budget Shoppers are the youngest and most price-sensitive segment —
  good fit for budget-friendly, trend-driven products.
- Average Middle-Class Shoppers show balanced behavior across all metrics —
  a stable general-purpose customer base.

## Tools Used
- Microsoft Power BI Desktop
- DAX for segment classification

## Files
- `Customer_Segmentation.pbix` – Power BI dashboard file
- `customer_data.xlsx` – Source dataset

## How to View
1. Download `Customer_Segmentation.pbix`
2. Open it in Power BI Desktop (free download from Microsoft)
3. Use the slicers to explore segments interactively
