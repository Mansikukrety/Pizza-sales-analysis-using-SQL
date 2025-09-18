🍕 Pizza Sales Analysis | SQL Data Exploration
📖 Project Overview
A comprehensive SQL analysis of a pizza restaurant's sales data to derive actionable business insights. This project focuses on understanding sales trends, customer preferences, and menu performance to support data-driven decision making for inventory management, marketing strategies, and operational efficiency.

🗄️ Database Structure
The database consists of four main tables in a relational schema:

orders: Contains order metadata (order_id, date)

order_details: Links orders to specific pizzas with quantities (order_details_id, order_id, pizza_id, quantity)

pizzas: Contains product details (pizza_id, pizza_type_id, size, price)

pizza_types: Describes pizza attributes (pizza_type_id, name, category, ingredients)

🛠️ Technical Stack
SQL (PostgreSQL compatible)

Data Analysis & Query Optimization

Git for version control

🔍 Key Analysis Areas
Revenue Analysis: Total revenue generation and performance metrics

Product Performance: Identification of best and worst-selling pizzas

Category & Size Analysis: Sales trends across different pizza categories and sizes

Temporal Patterns: Peak ordering hours and busiest days analysis

Menu Optimization: Identifying low-performing items for strategic review

📊 Key Insights
Classic category pizzas dominated in order volume and consistent popularity

Large-sized pizzas contributed significantly to overall revenue

Evening hours (6-9 PM) showed peak demand, aligning with dinner time

Several pizzas contributed less than 1% of total revenue, indicating potential menu optimization opportunities

🚀 Business Impact
The insights from this analysis can drive:

Inventory Management: Optimize stock levels based on popular items

Staffing Decisions: Align schedules with peak ordering times

Marketing Strategies: Focus promotions on high-margin items

Menu Engineering: Consider removing or repositioning low-performing items
