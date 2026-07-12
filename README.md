# 🍕 Pizza Sales Analytics — SQL Server & Power BI

An end-to-end data analytics project analyzing a year of pizza sales data (Jan–Dec 2015) using SQL Server (SSMS) for KPI extraction and Power BI for interactive dashboard visualization.

## 📊 Project Overview

This project answers key business questions about sales performance, customer ordering patterns, and product performance using a relational pizza sales dataset. It combines SQL-based analysis with a two-page interactive Power BI dashboard.

## 🎯 Key Metrics

- Total Revenue: $817,860
- Total Orders: 21,350
- Average Order Value: $38
- Avg Pizzas per Order: 2
- Total Pizzas Sold: 49,574

## 🛠️ Tools & Tech

- SQL Server Management Studio (SSMS)
- Power BI Desktop
- Microsoft Excel (data source)

## 🔍 Analysis Breakdown

A. Key Performance Indicators (KPIs)
- Total Revenue — SUM(total_price) → $817,860.05
- Average Order Value — SUM(total_price)/COUNT(order_id) → $16.82
- Total Pizzas Sold — SUM(quantity) → 49,574
- Total Orders — COUNT(DISTINCT order_id) → 21,350
- Avg Pizzas Per Order — SUM(quantity)/COUNT(DISTINCT order_id) → 2

B. Daily Trends for Total Orders
- Orders grouped by DATENAME(DW, order_date)
- Peak day: Friday (3,538 orders); lowest: Sunday (2,624 orders)

C. Monthly Trends for Total Orders
- Orders grouped by DATENAME(Month, order_date)
- Peak month: July (1,935 orders); lowest: February (1,685 orders)

D. % of Total Sales by Category
- Revenue and percentage share grouped by pizza_category
- Classic leads at 26.7% ($18,619.40), followed by Supreme (25.7%), Veggie (24.4%), Chicken (23.2%)

E. % of Total Sales by Size
- Revenue and percentage share grouped by pizza_size
- Large (L) dominates at 46.37% ($95,229.70), followed by Medium (29.78%), Small (22.10%), XL (1.60%), XXL (0.14%)

F. Top 5 Pizzas by Revenue
- Led by The Thai Chicken Pizza ($43,434.25), followed by Barbecue Chicken, California Chicken, Classic Deluxe, Spicy Italian

G. Bottom 5 Pizzas by Revenue
- Lowest: The Brie Carre Pizza ($11,588.50), followed by Green Garden, Spinach Supreme, Mediterranean, Spinach Pesto

H. Top 5 Pizzas by Quantity Sold
- Led by The Classic Deluxe Pizza (2,453 units), followed by Barbecue Chicken, Hawaiian, Pepperoni, Thai Chicken

I. Bottom 5 Pizzas by Quantity Sold
- Lowest: The Brie Carre Pizza (490 units), followed by Mediterranean, Calabrese, Spinach Supreme, Soppressata

J. Top 5 Pizzas by Order Count
- Led by The Classic Deluxe Pizza (2,416 orders), followed by Barbecue Chicken, Hawaiian, Pepperoni, Thai Chicken

K. Bottom 5 Pizzas by Order Count
- Lowest: The Brie Carre Pizza (480 orders), followed by Mediterranean, Calabrese, Spinach Supreme, Soppressata
  
## 📈 Dashboard Highlights

<img width="857" height="469" alt="Pizza Sales Dashboard Home" src="https://github.com/user-attachments/assets/b69a5d6e-8fa6-41ee-82c2-7db15360fe1d" />

Page 1 — Home: Revenue, orders, and pizza-sold trends by day/month, category and size breakdowns.

<img width="866" height="469" alt="best worst seller dashboard pizza" src="https://github.com/user-attachments/assets/7b808794-2179-4c66-8eda-208d4cd64753" />

Page 2 — Best/Worst Sellers: Top and bottom performing pizzas by revenue, quantity, and order count.

Key Insights:

- Classic category & Large size pizzas drive the most sales
- Order volume peaks on Fridays/Saturdays and in July/January
- The Thai Chicken Pizza leads in revenue; The Brie Carre Pizza underperforms across all metrics
