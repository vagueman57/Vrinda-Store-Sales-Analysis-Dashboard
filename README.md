# Vrinda Store Sales Data Analysis (Excel Project)

## Overview

This project analyzes sales data for Vrinda Store using Microsoft Excel. The primary goal was to extract actionable business insights to guide future marketing and sales strategies. The project incorporates data cleaning, processing, and comprehensive data analysis using Excel formulas and pivot tables.

---

## Dashboard

Below is the interactive dashboard generated from the analysis:

<img width="1743" height="684" alt="Screenshot 2026-05-27 181018" src="https://github.com/user-attachments/assets/356dea38-b1d9-4ec4-b1d9-38322dc8d318" />

*Vrinda Store Annual Report 2022 Dashboard*

---

## Objectives

The key questions addressed in this analysis:

1. **Month-wise sales and total orders**  
2. **Identify the month with highest sales and orders**
3. **Compare shopping patterns between men and women**
4. **Analyze order statuses**
5. **List top 5 states by sales**
6. **Breakdown sales and order count by gender**
7. **Determine the sales channel contributing most to overall sales**

---

## Project Workflow

### 1. Data Cleaning

- The original dataset had inconsistent gender notations: `M`, `W`, `Men`, `Women`.
- Standardized gender column using filter and replace functions to keep only `Men` and `Women`.

### 2. Data Processing

- **Age Group Segmentation:**  
  Age data was categorized as follows:
  ```
  =IFS(E2>=65, "Senior", E2>=40, "Middle-Aged Adult", E2>=20, "Young Adult", E2>=13, "Teens", TRUE, "Children")
  ```
  | Age Range | Group                |
  |-----------|----------------------|
  | >65       | Senior               |
  | 40-65     | Middle-Aged Adult    |
  | 20-39     | Young Adult          |
  | 13-19     | Teen                 |
  | <13       | Children             |

- **Extracting Month from Dates:**  
  To analyze month-wise data:
  ```
  =TEXT(G2, "mmm")
  ```

### 3. Data Analysis

- Used **Pivot Tables** to summarize data and create charts for:
  - Month-wise sales and order count
  - Top states by sales
  - Gender and age group analyses
  - Channel-wise contribution

- Inserted **Slicers** to add interactivity by filtering on:
  - Month
  - Sales Channel
  - Product Category

---

## Main Insights

- **Women make up 64% of buyers** — indicating women are more likely to make purchases at Vrinda Store.
- **Top 3 States:** Maharashtra (2.99M), Karnataka (2.65M), and Uttar Pradesh (2.10M) generate the most orders.
- **Age Group:** The 30-49 age bracket (Adults) contributes the majority of sales (Middle-Aged Adult + Young Adult = major share).
- **Sales Channels:** Amazon (35%), Flipkart (22%), and Myntra (23%) collectively account for 80% of sales.
- **Order Status:** 92% of the orders are delivered, with only 3% returned, 3% cancelled, and 2% refunded.
- **Month with Highest Sales:** [Please fill in based on your dataset; visible in the Orders vs Sales chart.]
- **Top 5 States by Sales:**  
  1. Maharashtra  
  2. Karnataka  
  3. Uttar Pradesh  
  4. Telangana  
  5. Tamil Nadu

---

## Visuals

Key plots included in the dashboard:
- Orders vs Sales (monthly trend)
- Sales by Men vs Women
- Order Status distribution (overall, and by channel)
- Sales: Top 5 States
- Orders: Age vs Gender

---

## Recommendations

Based on the above analysis, to boost Vrinda Store’s sales:

- **Target Audience:**  
  Focus marketing on **women aged 30-49**.

- **Geo-targeting:**  
  Prioritize advertising in **Maharashtra, Karnataka, and Uttar Pradesh**.

- **Channel Strategy:**  
  Invest more in visibility and offers on leading platforms: **Amazon, Flipkart, and Myntra**.

- **Promotional Tactics:**  
  Use ads, exclusive offers, and coupons tailored to women in the 30–49 age group on these channels to maximize conversion.

---

## Excel Features Used

- Data Cleaning with filters and Replace
- Advanced Formulas: `IFS`, `TEXT`
- Pivot Tables & Pivot Charts
- Slicers for interactive dashboards

---

## How to Use

1. Download/open the Excel file.
2. Explore the dashboards and slicers for month, channel, and category.
3. Review the charts and pivot tables for detailed insights.

---


## License

This analysis is for academic, learning, and internal usage. Please contact the author for commercial or public use.
