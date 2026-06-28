# Sales Performance Dashboard – Part 1

## Problem Summary

The objective of this project is to clean, validate, and analyze a retail sales dataset using Microsoft Excel. The project focuses on improving data quality, applying business rules, creating calculated columns, and producing pivot reports and a dashboard for business analysis.

---

## Dataset Description

The dataset contains customer order information including:

- Order ID
- Order Date
- Ship Date
- Customer Information
- Region
- Category
- Ship Mode
- Sales
- Cost
- Discount
- Profit
- Order Status

The raw dataset contains missing values, invalid records, duplicate IDs, incorrect dates, and inconsistent data that required cleaning before analysis.

---

## Tools Used

- Microsoft Excel
- Excel Formulas
- Pivot Tables
- Pivot Charts
- GitHub

---

## Cleaning Steps Performed

The following cleaning tasks were completed:

- Filled missing Region values with **"Unknown"**
- Filled missing Ship Mode values with **"Unknown"**
- Replaced missing Discount values with **0**
- Flagged negative Discount values
- Flagged Discounts greater than 50%
- Flagged invalid dates
- Flagged Ship Dates before Order Dates
- Flagged duplicate Order IDs
- Removed exact duplicate rows (none found)
- Excluded cancelled and failed payment orders from completed sales analysis
- Created calculated columns:
  - Calculated Sales
  - Calculated Profit
  - Profit Margin
  - Shipping Delay Days
  - Order Month

---

## Business Rules Applied

- Missing Region → Unknown
- Missing Ship Mode → Unknown
- Missing Discount → 0
- Negative Discounts are invalid
- Discounts above 50% are flagged
- Ship Date cannot be earlier than Order Date
- Duplicate Order IDs are flagged
- Cancelled and Failed Payment orders are excluded from completed sales reporting

---

## Summary of Data Quality Issues Found

| Issue | Count |
|-------|------:|
| Missing Region | 25 |
| Missing Ship Mode | 21 |
| Missing Discount | 38 |
| Negative Discount | 15 |
| Discount Above 50% | 7 |
| Invalid Dates | 257 |
| Ship Date Before Order Date | 4 |
| Duplicate Order IDs | 4 |
| Cancelled Orders | 145 |
| Returned Orders | 163 |
| Failed Payments | 69 |

---

## Summary of Pivot Reports

The project includes PivotTables for:

- Sales by Category
- Sales by Region
- Monthly Sales Trend
- Sales by Ship Mode
- Profit by Category
- Orders by Status

These PivotTables were used to build the final dashboard.

---

## Key Business Insights

- Technology generated the highest total sales.
- Office Supplies generated the lowest sales.
- South region recorded the highest sales among known regions.
- Standard Class was the most frequently used shipping method.
- Completed orders represented the majority of all orders.
- Monthly sales fluctuated throughout the year with several peak months.

---

## Assumptions and Limitations

- Missing categorical values were replaced with "Unknown".
- Missing Discount values were assumed to be zero.
- Flagged records were retained for reporting purposes.
- The analysis is based only on the provided dataset.

---

## Screenshots Included

The repository includes screenshots of:

- Raw dataset preview
- Cleaned dataset preview
- Pivot summary reports
- Dashboard

---

## Repository Structure

```
data/
outputs/
screenshots/
README.md
```
