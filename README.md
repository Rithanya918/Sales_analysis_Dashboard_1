# Pizza Sales Report 

## Project Overview

This project involves end-to-end analysis of pizza sales data using SQL (MySQL Workbench & Snowflake) and Tableau for data visualization. The goal is to analyze key business performance indicators, identify trends, and provide actionable insights based on real sales data from January 1, 2015 to December 31, 2015.

---

## Problem Statement

### KPI Requirements

We need to analyze key indicators for our pizza sales data to gain insights into our business performance. Specifically, we calculated the following metrics:

1. **Total Revenue** — The sum of the total price of all pizza orders.
2. **Average Order Value** — The average amount spent per order, calculated by dividing the total revenue by the total number of orders.
3. **Total Pizzas Sold** — The sum of the quantities of all pizzas sold.
4. **Total Orders** — The total number of orders placed.
5. **Average Pizzas Per Order** — The average number of pizzas sold per order, calculated by dividing the total number of pizzas sold by the total number of orders.

---

### Charts Requirements

We visualized various aspects of the pizza sales data to gain insights and understand key trends. The following charts were created:

1. **Hourly Trend for Total Orders** — A stacked bar chart displaying the hourly trend of total orders over the year to identify patterns or fluctuations in order volumes on an hourly basis.
2. **Weekly Trend for Total Orders** — A line chart illustrating the weekly trend of total orders throughout the year to identify peak weeks or periods of high order activity.
3. **Percentage of Sales by Pizza Category** — A pie/donut chart showing the distribution of sales across different pizza categories to provide insights into category popularity and contribution to overall sales.
4. **Percentage of Sales by Pizza Size** — A pie chart representing the percentage of sales attributed to different pizza sizes to understand customer preferences and their impact on sales.
5. **Total Pizzas Sold by Pizza Category** — A funnel chart presenting the total number of pizzas sold for each pizza category to compare sales performance across categories.
6. **Top 5 Best Sellers by Revenue, Total Quantity, and Total Orders** — A bar chart highlighting the top 5 best-selling pizzas to identify the most popular pizza options.
7. **Bottom 5 Best Sellers by Revenue, Total Quantity, and Total Orders** — A bar chart showcasing the bottom 5 worst-selling pizzas to identify underperforming or less popular options.

---

## Tools & Technologies Used

| Tool | Purpose |
|------|---------|
| MySQL Workbench | Initial data querying and KPI calculations |
| Snowflake | Cloud-based data warehousing and loading |
| Tableau | Dashboard creation and data visualization |
| CSV (pizza_data.csv) | Raw data source |

---

## KPI Results (Dashboard Summary)

| KPI | Value |
|-----|-------|
| Total Revenue | $817.9K |
| Average Order Value | $38.31 |
| Total Pizzas Sold | 49,574 |
| Total Orders | 21,350 |
| Avg Pizzas Per Order | 2.32 |

---

## Dashboard Pages

### Page 1 — Home (Sales Overview)
Covers hourly and weekly trends, sales by category and size, and total orders vs. pizzas sold by category.
https://github.com/user-attachments/assets/df355b8e-0a5f-4bee-a7ca-ac4606fcb975

### Page 2 — Best & Worst Sellers
Covers Top 5 and Bottom 5 pizzas by Revenue, Quantity, and Total Orders.
https://github.com/user-attachments/assets/122ddaf4-0ca3-40dc-b813-6d92171858ad
---

## Key Findings

- Peak order hours are **12PM–1PM** and **4PM–7PM**
- Highest weekly orders recorded in **Week 48 (491 orders)**; lowest at **Week 52 (171 orders)**
- **Classic category** leads in total orders and revenue ($220K, 26.9%)
- **Large size** pizzas dominate sales across all categories
- **Thai Chicken Pizza** is the #1 performer by revenue ($43,434) and total orders (2,225)
- **Brie Carre Pizza** is the lowest performer across all three metrics

---

## Project Structure

```
pizza-sales-project/
│
├── data/
│   └── pizza_data.csv              # Raw data file
│
├── sql/
│   ├── kpi_queries.sql             # SQL queries for all 5 KPIs
│   └── chart_queries.sql           # SQL queries for all 7 chart requirements
│
├── tableau/
│   ├── pizza_sales_home.png        # Dashboard Page 1 screenshot
│   └── pizza_sales_sellers.png     # Dashboard Page 2 screenshot
│
└── README.md                       # Project documentation
```

---

## How to Reproduce

1. Import `pizza_data.csv` into MySQL Workbench or Snowflake
2. Run the KPI SQL queries to validate the metrics
3. Run the chart SQL queries to generate data for visualizations
4. Connect Tableau to your database and build the dashboards using the chart requirements above

---

## Author

**Rithanya Sekar**
Data Analytics Project | 2015 Pizza Sales Analysis
