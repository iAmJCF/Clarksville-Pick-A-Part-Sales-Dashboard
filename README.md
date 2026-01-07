# Clarksville Pick A Part – Sales Intelligence Dashboard

## Business Context

Clarksville Pick A Part is a fictional auto salvage operation with three regional lots. Vehicles are purchased, placed on outdoor lots, and customers remove parts for purchase. The business operates year-round, including through weather events that impact customer activity.

## Business Objectives

The goal of this dashboard was to provide leadership with operational insight into:

- Revenue trends (Month-over-Month and Year-over-Year)
- Most profitable days of the week
- Top-performing vehicles and part categories
- Average time to profitability per vehicle
- Impact of extreme weather days (defined as $0 sales days)

## Solution Overview

This dashboard was designed and built in Power BI using normalized data modeled in MySQL and populated with generated sales data. Features include:

- Three years of historical sales data (2021–2023)
- Relational data model: customers, vehicles, parts, sales, weather
- Power BI report with:
  - Dynamic KPIs: Revenue, MoM/YoY trends, Days to Profit
  - Top vehicles and part sales
  - Daily sales analysis and weather overlay
- Row-Level Security (RLS) for:
  - District Manager (full visibility)
  - Lot Managers (Lot1, Lot2, Lot3 access only)
- Clean, branded layout styled in Austin Peay University colors (maroon and gray)

## Tools & Technologies

| Tool       | Purpose                        |
|------------|--------------------------------|
| Power BI   | Data modeling, DAX, dashboard  |
| MySQL      | Schema design, data integration |
| Python     | Dummy data generation          |
| DAX        | KPI calculations, RLS logic    |

## Files

- `Clarksville_Pick_A_Part.pbix` – Main Power BI dashboard
- `vehicles.csv`, `parts.csv`, `sales.csv`, `customers.csv`, etc. – Data sources
- `README.md` – Project documentation
- Optional: `demo.mp4` or screenshots for preview

## Getting Started

1. Download the `.pbix` file and open it in Power BI Desktop
2. All data is sourced from local CSVs, so no external connections are required
3. Review and test RLS roles via Modeling > View As Roles

## License

This project is for portfolio and educational use only. All data is fictional and generated.

## Author

Project created by Jerrod Frances as a professional portfolio piece.