# Delhivery-Logistics-Analytics

The firm wants to find opportunities to improve efficiency in operations and understand how the estimated delivery time/distance varies with respect to the actual delivery time/distance.

## 📅 Project Overview

This repository contains a Business Intelligence and Predictive Analytics project focused on enhancing the **logistics efficiency** of **Delhivery**, a leading supply chain company in India. The goal is to analyze delivery data, clean and preprocess it, and build an interactive dashboard and predictive model that provides insights into:
- Trip efficiency
- Route optimization
- Transportation types
- Overall delivery performance

## 📊 Objectives

1. **Data Cleaning and Preprocessing:** Handle missing values, convert types, and extract time-based features.
2. **Trip Efficiency Analysis:** Study patterns in trip durations and delays.
3. **Route Optimization Insights:** Analyze delivery routes to recommend better alternatives.
4. **Delivery Performance Metrics:** Track key performance indicators (KPIs).
5. **Forecasting Support:** Enable predictive models for delivery time estimation.

## :chart_with_upwards_trend: Dashboards

### 1. Trip Efficiency Dashboard

<p align="center">
<img src="./Media%20Github/Picture1.png" alt="Dashboard 1" width="500"/>
</p>

**KPIs and Metrics Tracked:**

- Average Trip Duration: The average time taken to complete a delivery trip, calculated from the trip start time to the trip end time.  
  Formula: Average (Trip End Time - Trip Start Time)
- Actionable Insights: Longer durations may indicate route inefficiencies or traffic bottlenecks.

### 2. Delivery Performance Dashboard

The number of deliveries that were completed successfully.

<p align="center">
<img src="./Media%20Github/Dashboard2.png" alt="Dashboard 2" width="500"/>
</p>

**KPIs and Metrics Tracked:**

- Total Deliveries Completed: The total number of successful deliveries within a given period.
- Actionable Insights: Spikes or drops in delivery volume can inform strategic decisions like hiring, route expansion, or operational changes.

### 3. Cost and Resource Utilization Dashboard

To analyze transportation costs, fuel efficiency, and resource utilization to enhance operational efficiency and optimize logistics expenditures.

<p align="center">
<img src="./Media%20Github/Dashboard3.png" alt="Dashboard 3" width="500"/>
</p>

**KPIs and Metrics Tracked:**

- Total Transportation Cost: The total cost incurred for transportation over a selected period.  
  Formula: Sum of all transport-related expenses  
- Actionable Insight: High overall cost prompts deeper analysis into specific cost drivers and enables identification of cost-saving areas.

### 4. Delivery Efficiency and Route Optimization

It focuses on evaluating the delivery performance and optimizing routes using the available data. It aims to analyze trip timings, distances, and segment-level details to identify areas for improvement in efficiency and routing strategies.

<p align="center">
<img src="./Media%20Github/Dashboard4.png" alt="Dashboard 4" width="500"/>
</p>

**KPIs and Metrics Tracked:**

- Average Start-to-End Delivery Time: Average time taken to deliver goods from source to destination.  
  Formula: (Sum of start_scan_to_end_scan) / Total Trips  
- Actionable Insights: Extremely high average delivery time suggests delays in either transit or hub handling.

### 5. Trip Timing and Distance Analysis

It focuses on understanding the relationship between trip times and distances. It identifies patterns and potential bottlenecks in trips by analyzing actual versus planned metrics, helping Delhivery optimize trip schedules and improve accuracy in time estimates.

<p align="center">
<img src="./Media%20Github/Dashboard .png" alt="Dashboard 5" width="500"/>
</p>

**KPIs and Metrics Tracked:**

- Average Trip Duration (Hours): Average time taken to complete a trip. 
  Formula: (Sum of actual_time) / Total Trips  
- Actionable Insight: A very high value (418 hours) indicates major operational inefficiencies. This metric should be compared over time and across routes or vehicle types to isolate performance gaps.

### 6.  Route Type Performance Dashboard

It aims to analyze the performance of different route types, such as FTL (Full Truck Load) and Carting, to understand their efficiency, usage patterns, and their impact on trip metrics. This analysis helps identify the optimal transportation type for specific scenarios and improves logistics decision-making.

<p align="center">
<img src="./Media%20Github/Dashboard6.png" alt="Dashboard 6" width="500"/>
</p>

**KPIs and Metrics Tracked:**

- Total Trips by Route Type: The count of trips completed for each route type.
  Formula: Count(trip_uuid) grouped by route_type
- Actionable Insight: FTL (Full Truck Load) accounts for ~69% of trips, while Carting makes up ~31%. This helps in understanding operational volume and load balancing between route types and may guide capacity or vehicle allocation decisions.

## :file_folder: Dataset Description

The dataset comprises **14,817 unique trips** and **144,867 total rows**. It includes:

- 24 attributes:
  - 12 object/categorical columns
  - 11 numerical columns
  - 1 boolean column
- Target column: `actual_time` (in minutes)
- Format: CSV

---

## :mag_right: Business Intelligence KPIs

| KPI                | Description                                    |
|--------------------|------------------------------------------------|
| Avg Delivery Time   | Mean delivery duration                          |
| Trip Efficiency    | Ratio of OSRM vs Actual time                    |
| Delay Patterns     | By route, time of day, location                 |
| Mode Performance   | FTL vs Carting metrics                          |
| Route Volume       | Number of trips per route                        |
| Delay Trends       | Time-based or location-based delays             |

## Conclusion

This project delivered valuable insights into Delhivery's logistics operations by analyzing trip timings, delivery efficiency, cost control, and route performance. Detailed dashboards identified bottlenecks, inefficiencies, and opportunities to optimize costs and improve service. Using Power BI and Excel, advanced visualization and data preprocessing uncovered hidden patterns, empowering the team to make data-driven decisions. The outcomes support enhanced planning, better delivery adherence, cost reduction, and scalable growth.

## Final Takeaway

The analysis confirms that Full Truck Load (FTL) trips are the most cost-effective and reliable for long-distance deliveries. Dashboards highlighted significant delays and missed cutoffs that escalate time and expense, indicating areas for process improvement. Regional and temporal delay trends suggest targeted interventions can improve efficiency. Resolving data inconsistencies enabled metric creation, providing clearer visibility. These dashboards equip Delhivery for informed logistics decisions and future advancements, including predictive modeling with machine learning.

