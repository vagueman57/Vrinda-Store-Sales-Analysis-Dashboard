# Vrinda Store Sales Data Analysis (Excel Project)

## Overview

This project analyzes sales data for Vrinda Store using Microsoft Excel. The primary goal was to extract actionable business insights to guide future marketing and sales strategies. The project incorporates data cleaning, processing, and comprehensive data analysis using Excel formulas and pivot tables.

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

- **Women make up 65% of buyers** — indicating women are more likely to make purchases at Vrinda Store.
- **Top 3 States:** Maharashtra, Karnataka, and Uttar Pradesh generate 35% of all orders.
- **Age Group:** The 30-49 age bracket (Adults) contributes 50% of sales.
- **Sales Channels:** Amazon, Flipkart, and Myntra collectively account for 80% of sales.
- **Month with Highest Sales:** [Fill in based on your dataset]
- **Most Contributing Channel:** [Fill in based on your dataset or state Amazon/Flipkart/Myntra based on above insights]
- **Top 5 States by Sales:**  
  1. Maharashtra  
  2. Karnataka  
  3. Uttar Pradesh  
  4. Telangana
  5. 5. Tamil Nadu

---

## Order Status Analysis

-<img width="1743" height="689" alt="image" src="https://github.com/user-attachments/assets/e6841e74-90e1-4d8f-993c-8a01378b0ea8" />
 [Add a table/chart or brief summary of findings regarding the distribution of order statuses, e.g., Delivered, Returned, Pending]

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
