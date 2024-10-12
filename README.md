# AtliQ Mart Supply_Chain_Analysis

## Overview

This project focuses on analyzing supply chain performance for **Atliq Mart**, with three levels of analysis: **Order Level**, **Product Level**, and **Customer Level**. Key metrics such as **On-Time (OT%)**, **In-Full (IF%)**, and **On-Time In-Full (OTIF%)** are measured and compared to targets to assess supply chain efficiency.

The analysis identifies areas of improvement, delays, and potential production issues. The data includes customer orders, delivery dates, and targets, which are used to calculate performance metrics.

---

## Key Metrics

- **OT% (On-Time Percentage)**: Measures the percentage of orders delivered on time.
- **IF% (In-Full Percentage)**: Measures the percentage of orders delivered in full quantity.
- **OTIF% (On-Time In-Full Percentage)**: Measures the percentage of orders delivered both on time and in full.
- **ADDD (Average Delivery Delay Days)**: The average number of days delayed beyond the agreed delivery date.
- **POR (Perfect Order Rate)**: Measures the percentage of orders delivered without any issues (on-time, in-full, and with correct documentation).
- **OCT (Order Cycle Time)**: The average time (in days) taken from order placement to delivery.
- **OFR (Order Fill Rate)**: The percentage of total orders that were fulfilled completely.

---

## Key Insights

1. **Key Metrics Below Target**:
   - All key metrics (**OT%, IF%, and OTIF%**) are underperforming and are far below the target levels.
   
2. **Average Delivery Delay**:
   - Orders are delayed by an average of **1.69 days**, which indicates inefficiency in meeting agreed delivery dates.
   
3. **Perfect Order Rate**:
   - Only **29%** of orders are delivered perfectly (on-time, in-full, and correct documentation), indicating frequent fulfillment issues.
   
4. **Order Cycle Time**:
   - The average time to complete an order is **4.85 days**, which can be optimized for faster deliveries.
   
5. **Order Fill Rate**:
   - **96.59%** of orders are fulfilled completely, with a shortfall in **3.41%** of orders.

---

## Analysis Breakdown

### 1. **Order Level Analysis**
   - **Charts**: 
     - Order Trends (e.g., Total Orders, Delayed Orders)
     - Order Delivery Performance (OT%, IF%, OTIF%)
   - **Metrics**: 
     - OT%, IF%, OTIF%, OCT, ADDD, POR

### 2. **Product Level Analysis**
   - **Charts**:
     - Product Delivery Delays (Most Delayed Products)
     - Product Order Performance (OTIF% per Product)
   - **Metrics**:
     - Product-wise OT%, IF%, OTIF%, and ADDD

### 3. **Customer Level Analysis**
   - **Charts**:
     - Top Customers by Order Volume
     - Delayed Orders by Customer
   - **Metrics**:
     - Customer-wise OT%, IF%, OTIF%, and ADDD

---

## Key Observations

- **Lotus Mart, Coolblue, and Acclaimed Stores**: Highest order volume but also the most delayed deliveries.
- **Ghee, Curd, and Butter**: Most delayed products in terms of delivery.
- **Production Issues**: Large gaps in IF% may be due to insufficient production capacity.
- **No noticeable improvements**: Metrics show no improvement over recent months, indicating a need for operational adjustments.

---

## Next Steps

1. **Improve Delivery Planning**: Reassess delivery dates to better estimate order timelines.
2. **Increase Production Capacity**: Address production bottlenecks to meet demand.
3. **Optimize Fulfillment Processes**: Implement strategies to improve OTIF% and minimize delays.

---

## Data Sources

- **dim_customers**: Contains customer information (e.g., customer_id, customer_name, city).
- **dim_products**: Contains product information (e.g., product_name, product_id, category).
- **dim_date**: Contains date information (e.g., date, mmm_yy, week_no).
- **dim_targets_orders**: Contains customer-level targets for On-Time, In-Full, and OTIF%.
- **fact_order_lines**: Contains order line information (e.g., order_id, customer_id, product_id, order_qty, delivery dates).
- **fact_orders_aggregate**: Aggregated order information for On-Time, In-Full, and OTIF.

---

## Tools Used

- **Microsoft Power BI**: For visualizing the data and creating the dashboard.
- **DAX**: Used to create calculated measures and columns for the analysis.
- **M Language**: Applied for transformations in Power Query Editor.

