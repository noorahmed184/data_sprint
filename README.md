# data_sprint
# Olist Sales Performance & Resources

## Problem Statement

Olist is a Brazilian e-commerce marketplace connecting sellers with customers across Brazil. This project analyzes Olist's sales performance from 2016 to 2018 to understand revenue trends, customer and seller activity, product performance, purchasing patterns, and opportunities for increasing sales.

---

## Executive Summary

This project analyzes Olist's e-commerce sales performance using transactional data covering approximately 2016–2018. The analysis combines multiple datasets, including orders, order items, customers, sellers, products, payments, and product categories. The data was cleaned and integrated to create a final analytical dataset suitable for exploring sales trends, order performance, customer behavior, product categories, geographic patterns, and purchasing characteristics.

Exploratory Data Analysis (EDA) was used to investigate overall sales performance, monthly and yearly sales growth, average order value, peak purchasing periods, sales by weekday and hour, product-category performance, customer and seller locations, payment methods, installments, and other factors related to marketplace performance. Engineered features such as sales, year, month, weekday, hour, and translated product categories were used to support the analysis.

The analysis identified clear patterns in Olist's sales performance, including changes in sales over time and seasonal purchasing patterns. Sales performance also varies substantially across product categories and geographic markets. These findings can help Olist identify high-performing product categories, understand when customer demand is strongest, and focus resources on opportunities that can increase sales and marketplace activity.

---

# Data and Data Dictionary

## Data Source

The dataset used in this project is the **Brazilian E-Commerce Public Dataset by Olist**, which contains anonymized information about orders made through the Olist marketplace in Brazil.

The dataset contains information about orders, customers, sellers, products, payments, reviews, and product categories. The data covers approximately **2016 to 2018**.

**Source:** Olist Brazilian E-Commerce Public Dataset
**Source link:** https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

---

## Dataset Overview
The Olist dataset contains approximately **100,000 orders**, with multiple records associated with individual orders because one order can contain multiple products and payment transactions.

---

# Final Cleaned Dataset

The final analytical dataset combines relevant information from the original Olist tables to support sales-performance analysis, focused on Jan 2017 - Aug 2018 period.

### Key Features

**Order information**

* `order_id`
* `customer_id`
* `order_status`
* `order_purchase_timestamp`
* `order_approved_at`
* `order_delivered_carrier_date`
* `order_delivered_customer_date`
* `order_estimated_delivery_date`

**Customer information**

* `customer_unique_id`
* `customer_zip_code_prefix`
* `customer_city`
* `customer_state`

**Seller information**

* `seller_id`
* `seller_zip_code_prefix`
* `seller_city`
* `seller_state`

**Product information**

* `product_id`
* `product_category_name`
* `product_category_name_english`
* `product_weight_g`
* `product_length_cm`
* `product_height_cm`
* `product_width_cm`

**Sales and payment information**

* `order_item_id`
* `price`
* `freight_value`
* `payment_type`
* `payment_installments`
* `payment_value`

---

# Exploratory Data Analysis

The analysis focuses on answering the client's key sales-performance questions.

## 1. Overall Sales Performance

The analysis examines:

* Total sales
* Number of orders
* Number of customers
* Sales growth over time 610.3%

### Key Findings

* Total sales: **[13.5 million]**
* Total orders: **[99 thousand]**
* Average Order Value: **[92 thousand]**
* Sales growth from the first month to the final month: **[610.3 %]**

---

## 2. Sales Trends Over Time

Monthly and yearly sales were analyzed to identify changes in marketplace performance.

The analysis found that sales generally increased as the marketplace developed, although monthly fluctuations were present.

### Key Findings

* Highest-sales month: **[November]**
* Lowest-sales month: **[January]**
* Highest-sales year: **[2018]**

Seasonal patterns were also examined to identify periods of particularly strong or weak customer demand.

---

## 3. Customer and Order Performance

Customer activity was analyzed using order counts and purchasing behavior.

The analysis examines:
* Average order value

### Key Finding

**[Growth Came From More Orders, Not Bigger Baskets]**

---

## 4. Product Category Performance

Product categories were analyzed to determine which categories contribute the most to sales.

The analysis compares categories based on:

* Total sales
* Number of orders/items sold
* Average item price
* Customer demand

### Key Findings

* Top category by sales: **[INSERT CATEGORY]**
* Top category by number of items/orders: **[INSERT CATEGORY]**
* Lowest-performing category: **[INSERT CATEGORY]**

These differences indicate that sales volume and sales value do not necessarily follow the same pattern across categories.

---

## 5. Sales by Day and Time

Order timestamps were used to investigate when customers are most active.

The analysis examines:

* Sales by weekday
* Sales by hour
* Peak purchasing periods

### Key Findings

* Highest-sales weekday: **[Monday]**
* Peak purchasing hour: **[Morning at 10am]**

These patterns can help Olist optimize marketing campaigns and promotional timing.

---

## 6. Geographic Performance

Customer and seller locations were analyzed to understand the geographic distribution of Olist's marketplace activity.

The analysis examines:

* Sales by customer state
* Customer concentration
* Seller concentration
* States with customers but limited seller presence

### Key Finding

**[INSERT MAIN GEOGRAPHIC INSIGHT]**

---

## 7. Payment and Purchasing Behavior

Payment information was analyzed to understand how customers pay for their purchases.

The analysis examines:

* Payment methods
* Payment values
* Installment behavior
* Relationship between payment methods and order value

### Key Findings

* Most common payment method: **[INSERT METHOD]**
* Most common number of installments: **[INSERT NUMBER]**
* Average payment/order value: **[INSERT VALUE]**

---

# Conclusions and Recommendations

The analysis shows that Olist's sales performance is influenced by several factors, including time of purchase, product category, customer geography, and purchasing behavior.

### Recommendations

1- To increase the AOV: Create product bundles

2- To incraese Revenues: Focus on Retention (Repeat Buyers), As we have 92K customers but 99K orders.

3- Target the Monday/Tuesday Afternoon Shoppers 

 4- Launch a "Black November" campaign, give your 92K existing customers early access, and promote high value bundles.

5- Prioritize seller recruitment in states with low seller coverage.

6- Provide onboarding incentives for new sellers.

7- Focus marketing and inventory efforts on the product categories that generate the highest sales.

8-Monitor the impact of discounts, vouchers, and installments to identify which strategies are associated with better sales performance

---

# Areas for Further Research / Study

Future analysis could investigate:

* Customer retention and repeat-purchase rates
* Seller performance and seller retention
* Profitability rather than sales revenue alone
* Relationship between delivery performance and customer reviews
* Product pricing and demand
* Discounts and promotional effects
* Customer segmentation
* Predictive sales forecasting
* Marketplace commission/revenue modeling

A future project could also develop predictive models to forecast sales or classify customers based on purchasing behavior.

---

# Sources

* Olist Brazilian E-Commerce Public Dataset — Kaggle
* Olist dataset documentation and original dataset tables
* Any additional external sources used for market or business context: **[ADD SOURCES HERE]**

---

# Project Scope

This project focuses on **descriptive and exploratory analysis of Olist's sales performance**. Machine learning modeling is not included because the primary objective is to understand historical sales patterns and generate actionable business recommendations from the available data.
