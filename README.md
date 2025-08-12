# Sales Trend Analysis (Task 6 - Data Analyst Internship)

## Objective
Analyze **monthly revenue** and **order volume** from the `online_sales` dataset using SQL aggregation functions.

## Tools Used
- PostgreSQL (queries compatible with MySQL & SQLite)
- Dataset: `online_sales` table (columns: order_date, amount, product_id, order_id)

## Steps Performed
1. **Extracted** `year` and `month` from `order_date`.
2. **Grouped** data by `year` and `month`.
3. **Calculated**:
   - **Monthly Revenue** = `SUM(amount)`
   - **Order Volume** = `COUNT(DISTINCT order_id)`
4. **Sorted** results chronologically with `ORDER BY`.
5. Found **Top 3 months by revenue** using `ORDER BY monthly_revenue DESC LIMIT 3`.

## SQL Scripts
The `sales_trend.sql` file contains:
- Monthly sales trend query.
- Top 3 months by revenue query.

## Example Output
| year | month | monthly_revenue | order_volume |
|------|-------|-----------------|--------------|
| 2023 | 1     | 7319            | 7            |
| 2023 | 2     | 3085            | 4            |
| 2023 | 3     | 6136            | 8            |

**Top 3 Months by Revenue:**
| year | month | monthly_revenue |
|------|-------|-----------------|
| 2023 | 1     | 7319            |
| 2023 | 3     | 6136            |
| 2023 | 2     | 3085            |

---
