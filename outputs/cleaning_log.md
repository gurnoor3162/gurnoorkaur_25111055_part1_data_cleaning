# Cleaning Log

## Data Cleaning Steps

- Filled missing Region values with "Unknown"
- Filled missing Ship Mode values with "Unknown"
- Replaced missing Discount values with 0
- Flagged negative discount values
- Flagged discounts greater than 50%
- Flagged invalid order and ship dates
- Flagged duplicate Order IDs
- Removed exact duplicate rows (none found)
- Excluded failed payments and cancelled orders from completed sales analysis
- Created calculated columns:
  - calculated_sales
  - calculated_profit
  - profit_margin
  - shipping_delay_days
  - order_month

Data quality report generated successfully.
