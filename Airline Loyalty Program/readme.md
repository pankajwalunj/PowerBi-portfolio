# Airline Loyalty Program Dashboard ✈️

An interactive Power BI dashboard analyzing customer engagement, flight activity, and lifetime value within an airline's loyalty rewards program.

![Dashboard Screenshot](images/dashboard_screenshot.png)

## Overview

This project explores customer-level data from an airline loyalty program, combining flight activity with customer demographics to understand how members engage with the program, how loyalty tiers differ in value, and how enrollment/cancellation trends have evolved over time.

## Key Features

- **Customer demographics breakdown** — by education, income, marital status, gender, and geography (country/province/city)
- **Loyalty tier analysis** — comparing Star, Nova, and Aurora tier members
- **Flight activity trends** — flights booked, distance traveled, and points earned/redeemed by month and year
- **Customer Lifetime Value (CLV)** — total invoice value per member, segmented by loyalty tier and enrollment type
- **Enrollment & cancellation trends** — enrollment type (Standard vs. 2018 Promotion) and cancellation patterns over time
- Built entirely in **Power BI Desktop** using a relational data model

## Data Model

The dashboard is built on three related tables:

| Table | Description |
|---|---|
| `Customer Flight Activity` | Monthly flight activity per customer — flights booked, distance, points accumulated/redeemed |
| `Customer Loyalty History` | Customer profile — demographics, loyalty card tier, CLV, enrollment and cancellation details |
| `Calendar` | Date table for time intelligence |

Full field-level definitions are in [`Airline_Loyalty_Data_Dictionary.csv`](Airline_Loyalty_Data_Dictionary.csv).

## Tech Stack

- **Power BI Desktop** — data modeling, DAX measures, and dashboard design
- **CSV** source data (customer flight activity, loyalty history, calendar)

## Repository Contents

```
├── Airline_Dashboard.pbix                    # Power BI dashboard file
├── Customer_Flight_Activity.csv
├── Customer_Loyalty_History.csv
├── Calendar.csv
├── Airline_Loyalty_Data_Dictionary.csv
├── images/                                    # Dashboard screenshot(s)
└── README.md
```

## How to Use

1. Clone this repo
2. Open `Airline_Dashboard.pbix` in [Power BI Desktop](https://www.microsoft.com/en-us/power-platform/products/power-bi/downloads) (free)
3. Use the dashboard filters/slicers to explore by loyalty tier, enrollment type, or time period
4. Review flight activity and CLV trends across customer segments

## Insights

- Loyalty tier (Star/Nova/Aurora) shows a clear relationship with customer lifetime value
- [Add your own takeaway here once you've explored further — e.g. enrollment trend post-2018 promotion, cancellation drivers, high-value customer segments]

## Author

Built by Pankaj Walunj as a data analytics/BI portfolio project.
