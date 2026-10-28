Retail Sales Dashboard | Power BI

An interactive Power BI report for exploring retail sales, product performance, profitability, promotions, and order details.

## Project overview

The report is organized into five pages:

- **Overview:** sales trend over time, sales and profit relationship, discount value by promotion, order count, and sales by city.
- **Top/Bottom 5 Analysis:** product rankings for sales, profit, and quantity sold.
- **Comparison Sales/Profit/Quantity Sold:** compare selected date periods across the three measures.
- **Edit Interactions:** a dedicated page for exploring visual interactions and period filters.
- **Table Visual:** order-level details with date, customer, product, promotion, sales, discount, profit, and quantity fields, with slicers for date, promotion, product, and customer.

## Business requirements covered

| Requirement | Report implementation |
|---|---|
| Top 5 and bottom 5 products by sales, profit, and quantity sold | Top/Bottom 5 Analysis page |
| Sales trends over time | Overview line chart by date |
| Sales and profit relationship | Overview scatter chart |
| Compare sales, profit, and quantity across two periods | Comparison page with two date slicers and measure visuals |
| Total discount value by promotion | Overview chart shows summed Discount Value by Promotion Name |
| Total number of orders | Overview order-count card using Order ID |
| Order-level details and filtering | Table Visual page with date, promotion, product, and customer slicers |
| Sales by city | Overview map using customer city |

## Data and measure notes

- The report model includes transaction fields for Order ID, CustomerID, PromotionID, Product ID, date, units sold, price per unit, total sales, discount percentage, discount value, net sales, and profit, plus customer, product, and promotion lookup tables.
- Confirm the definitions and source logic for **Profit**, **Net Sales**, **Discount Value**, and **Order Count** before publishing results. The report layout identifies these fields, but this README does not assert how their calculations were defined.
- The discount view reports the total Discount Value grouped by Promotion Name.
- Do not publish the original customer table if it contains names, emails, phone numbers, or other identifying data. Use sanitized or synthetic data in any public sample.

## Repository structure

```text
retail-sales-dashboard/
├── images/
│   └── dashboard-overview.png   # Screenshot with personal information removed
├── data/
│   └── README.md                # Data source and sanitization notes
├── README.md
```

Keep the `.pbix` file private if it embeds personal customer data. If you share a report file, first remove or replace identifying data and verify the published copy.

## Tools

- Microsoft Power BI
- Excel workbook source

## View the project

1. Open the sanitized `Sales Dashboard.pbix` file in Power BI Desktop.
2. Choose a page from the report tabs.
3. Use the slicers and visual interactions to filter and compare the data.

## Screenshot

Add a screenshot of the finished report after checking that no customer identifying information is visible.
