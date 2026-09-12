# Sales-Profitability-Analysis-Real-Dataset-

An exploratory data analysis (EDA) of a real retail sales dataset, examining performance across regions, sales reps, product categories, pricing, and time.

## About this project

This project applies pandas, matplotlib, and correlation analysis to a real-world sales dataset sourced from Kaggle. It builds on an earlier synthetic-data project by working with actual, externally-sourced business data — including calculated fields (profit, margin), datetime handling, and multi-column groupby analysis.

## Dataset

- Source: Kaggle — [add dataset link here]
- Columns: `Product_ID`, `Sale_Date`, `Sales_Rep`, `Region`, `Sales_Amount`, `Quantity_Sold`, `Product_Category`, `Unit_Cost`, `Unit_Price`, `Customer_Type`, `Discount`, `Payment_Method`, `Sales_Channel`

## Questions explored

1. Which region generates the highest total sales?
2. Which sales rep has the highest total sales?
3. Which product category sells the most units?
4. Which product category generates the highest revenue?
5. Which product category has the highest profit margin?
6. Which sales rep applies the highest average discount?
7. Is there a relationship between discount and profit?
8. Do New or Returning customers spend more on average?
9. Which payment method is used most often?
10. Which sales channel generates more revenue?
11–12. How do total sales trend by month, and which month peaks?
13. Which region-rep combination performs best?
14. Which region has the most New vs Returning customers?
15. Does a higher unit price correlate with lower quantity sold?

## Key takeaways

- North is the top-performing region by total sales (₦1,369,612.51), though all four regions are fairly close together.
- David is the top-performing sales rep by total sales (₦1,141,737.36), notably ahead of Charlie, the lowest performer.
- Clothing leads in both units sold and total revenue.
- Furniture has the highest average profit margin (₦261.65 per unit) despite not leading in volume or revenue — showing margin and volume don't always align.
- Credit Card is the most-used payment method (345 transactions), though no single method dominates heavily.
- No meaningful relationship was found between Discount and Sales_Amount (correlation = 0.023), nor between Unit_Price and Quantity_Sold (correlation = 0.057) — pricing and discounting do not appear to drive sales volume in this dataset.
- January was the peak month for total sales (₦495,420.37), with noticeable month-to-month volatility across the year rather than a steady trend.
- The split between New and Returning customers is fairly even across all four regions — no region stands out as disproportionately reliant on one customer type.

## Limitations

- This dataset does not include unique customer IDs, so total spend per individual customer cannot be calculated — only category-level (New vs Returning) comparisons are possible.
- Correlation only captures straight-line relationships; a genuine non-linear pattern (e.g. a "sweet spot" price point) could exist without showing a strong correlation number. Scatter plots were used alongside correlation to check for this.

## Tools used

- Python, pandas, matplotlib
- Jupyter Notebook

## Author

Chidera Enemuo — [github.com/chideraenemuo](https://github.com/chideraenemuo)
