create database pizzahut;
SELECT * FROM pizzahut;

CREATE table orders(
order_id int not null,
order_date date not null,
order_time time not null,
primary key(order_id));


CREATE table order_details(
order_details_id int not null,
order_id int not null,
pizza_id text not null,
quantity int not null,
primary key(order_details_id));-- List all unique pizza categories

SELECT DISTINCT category 
FROM pizza_types;

-- Count the total number of pizzas on the menu

SELECT COUNT(*) AS total_pizzas
FROM pizzas;

-- Show all pizza sizes available 

SELECT DISTINCT size
FROM pizzas;

-- Find total number of orders placed

SELECT COUNT(order_id) AS total_orders
FROM orders;

-- Find total no. of weekend orders( saturday+sunday)

SELECT COUNT(*) AS weekend_orders
FROM orders
WHERE dayofweek(order_date) IN (1,7);

-- Total revenue generated from pizza sales

SELECT ROUND(SUM(od.quantity * p.price),0) AS total_revenue
FROM order_details od
JOIN pizzas p ON 
od.pizza_id = p.pizza_id;


