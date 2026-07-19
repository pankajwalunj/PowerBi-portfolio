# Toy Store Sales Dashboard 🧸

An interactive Power BI dashboard analyzing sales, revenue, profit, and inventory performance across toy store locations, built to surface trends by store type, product category, and time period.

![Dashboard Screenshot](images/dashboard_screenshot.png)

## Overview

This project explores retail performance data for a toy store chain with locations across four store-location types — **Airport, Commercial, Downtown, and Residential**. The dashboard lets users filter by location type and drill into orders, revenue, and profit trends over time, as well as performance by product category.

## Key Features

- **Location filter** — toggle between Airport, Commercial, Downtown, and Residential stores
- **KPI cards** — total orders, revenue, and profit for the selected filter
- **Orders by product category** — bar chart comparing Toys, Art & Crafts, Games, Sports & Outdoors, and Electronics
- **Revenue trend** — monthly revenue line chart from Jan 2022–2023, highlighting seasonal peaks
- Built entirely in **Power BI Desktop** using a star-schema data model

## Data Model

The dashboard is built on five related tables:

| Table | Description |
|---|---|
| `Sales` | Transaction-level sales records (Sale ID, Date, Store ID, Product ID, Units) |
| `Products` | Product catalog with category, cost, and retail price |
| `Stores` | Store metadata — name, city, location type, open date |
| `Inventory` | Stock on hand by store and product |
| `Calendar` | Date table for time intelligence |

Full field-level definitions are in [`data/data_dictionary.csv`](data/data_dictionary.csv).

## Tech Stack

- **Power BI Desktop** — data modeling, DAX measures, and dashboard design
- **CSV** source data (sales, products, stores, inventory, calendar)

## Repository Contents

```
├── Toy_Store_Dashboard.pbix     # Power BI dashboard file
├── data/                        # Source data tables
├── images/                      # Dashboard screenshot(s)
└── README.md
```

## How to Use

1. Clone this repo
2. Open `Toy_Store_Dashboard.pbix` in [Power BI Desktop](https://www.microsoft.com/en-us/power-platform/products/power-bi/downloads) (free)
3. Use the Store Location buttons at the top to filter the dashboard
4. Explore orders, revenue, and profit trends by category and month

## Insights

- Revenue shows a clear seasonal pattern, peaking around Jul–Aug before dipping into the fall
- Toys and Art & Crafts consistently lead order volume across categories
- [Add your own takeaway here once you've explored further]

## Author

Built by Pankaj Walunj as a data analytics/BI portfolio project.
