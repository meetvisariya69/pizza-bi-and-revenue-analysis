# Pizza Sales Performance & Revenue Analytics

## Project Overview
This project focuses on extracting actionable business insights from a pizza restaurant's sales data using SQL. The analysis progresses from foundational data aggregation to intermediate relational joins, culminating in advanced analytics (such as cumulative revenue tracking and category-specific rankings using window functions).

## Core Objectives
* **Sales Performance:** Identify top-performing products and overall revenue metrics.
* **Consumer Behavior:** Analyze peak ordering hours and daily ordering patterns to optimize kitchen operations.
* **Market Share:** Calculate percentage revenue contributions by pizza category to guide menu engineering.

## Dataset Structure
The project utilizes 4 interconnected CSV datasets (stored in the `/data` folder):
* `orders.csv`: Contains order IDs, dates, and timestamps.
* `order_details.csv`: Connects orders to specific pizzas, including quantities.
* `pizzas.csv`: Details specific pizza SKUs, sizes, and their respective prices.
* `pizza_types.csv`: Maps pizzas to their formal names, categories, and ingredients.

---

## Analytical Roadmap & SQL Queries

### Phase 1: Basic Operations
1. **Total Order Volume:** Retrieve the total number of orders placed.
2. **Gross Revenue:** Calculate the total revenue generated from pizza sales.
3. **Pricing Anchors:** Identify the highest-priced pizza.
4. **Size Demands:** Identify the most common pizza size ordered.
5. **Volume Leaders:** List the top 5 most ordered pizza types along with their quantities.

### Phase 2: Intermediate Insights
1. **Category Popularity:** Join tables to find the total quantity of each pizza category ordered.
2. **Hourly Traffic:** Determine the distribution of orders by hour of the day to identify peak operational hours.
3. **Menu Breakdown:** Join relevant tables to find the category-wise distribution of pizzas.
4. **Daily Averages:** Group orders by date and calculate the average number of pizzas ordered per day.
5. **Revenue Champions:** Determine the top 3 most ordered pizza types based on revenue.

### Phase 3: Advanced Business Intelligence
1. **Revenue Contribution:** Calculate the percentage contribution of each pizza type to total revenue.
2. **Growth Tracking:** Analyze the cumulative revenue generated over time.
3. **Category Rankings:** Determine the top 3 most ordered pizza types based on revenue for *each* pizza category using `DENSE_RANK()`.

---

## How to Run the Queries
1. Clone this repository.
2. Import the 4 CSV files located in the `/data` directory into your SQL database instance (e.g., MySQL, PostgreSQL).
3. Open `scripts/solutions.sql` to view and execute the corresponding queries.
