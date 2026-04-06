# 🛒 Olist E-Commerce Intelligence Dashboard
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Data Analytics](https://img.shields.io/badge/Data_Analytics-005571?style=for-the-badge)
![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)

An interactive Power BI dashboard analyzing massive volumes of decentralized e-commerce data from Olist (a major Brazilian e-commerce platform) over multiple years. Built as a Capstone Project under the **Microsoft Elevate x AICTE Internship program**.

---

## 📸 Dashboard Preview

### Page 1: Executive Overview
Designed for high-level stakeholders, tracking overarching KPIs against corporate targets.
* **Features:** Target-tracking Gauge Chart, seasonal Revenue Trendline, and geographical sales density map.

![Overview Page](https://github.com/kuldeeprc2021-max/Olist-Ecommerce-Data-Analysis-Report-/blob/main/1774161719768.png)

### Page 2: Product Performance Deep-Dive
Built for inventory and supply chain managers to rapidly identify profitable items and dead stock.
* **Features:** Conditional Matrix formatting (Data Bars) and dynamic Top 10 / Bottom 10 Revenue Generator bar charts.

![Products Page](https://github.com/kuldeeprc2021-max/Olist-Ecommerce-Data-Analysis-Report-/blob/main/1774161720433.png)

### Page 3: Customer & Geographic Insights
Tailored for marketing and logistics teams to understand regional customer density.
* **Features:** Interactive bubble map of customer distribution, Treemap of top-performing cities, and month-over-month customer acquisition Area Chart.

![Customers Page](https://github.com/kuldeeprc2021-max/Olist-Ecommerce-Data-Analysis-Report-/blob/main/1774161721137.png)

---

## 💡 Key Findings

| Metric | Insight | Impact |
| :--- | :--- | :--- |
| **Top Revenue Drivers** | `beleza_saude` (Health & Beauty) and `cama_mesa_banho` (Bed/Bath) | Indicates where primary marketing budgets should be allocated. |
| **Regional Dominance** | Massive concentration in **São Paulo (SP)**. | Presents opportunities for localized distribution centers to reduce freight costs. |
| **Underperforming Stock** | Niche categories like `pc_gamer` rank in the bottom 10. | Highlights areas for immediate inventory reduction and purchasing halts. |

---

## 🗂️ Dataset Details
The project utilizes the Olist Brazilian E-Commerce Public Dataset, comprising multiple relational CSV files.

| Table | Records | Description |
| :--- | :--- | :--- |
| `olist_orders_dataset` | ~99,441 rows | Core order timestamps, delivery status, and unique order IDs. |
| `olist_order_items` | ~112,650 rows | Line items for each order including price and freight value. |
| `olist_products` | ~32,951 rows | Product catalog with category metadata and dimensions. |
| `olist_customers` | ~99,441 rows | Customer demographic and geographic spatial data (city, state). |

---

## ⚙️ Tech Stack & Methodology

| Component | Technology | Description |
| :--- | :--- | :--- |
| **Visualization** | Microsoft Power BI | Primary tool for dashboard UI/UX design. |
| **Data Transformation** | Power Query (M Language) | Handled null values, standardized currency, and engineered temporal features. |
| **Calculated Measures** | DAX | Engineered custom KPIs (Total Revenue, Distinct Customers, Freight Cost). |
| **Data Source** | CSV / Flat Files | Extracted via Kaggle Open Datasets. |

### 🗄️ Data Model
The dashboard is built on a **Star Schema** architecture. Central fact tables (`Orders`, `Order_Items`) are actively linked to dimension tables (`Customers`, `Products`) via one-to-many relationships, optimizing the VertiPaq engine for seamless, multi-page cross-filtering.

---
## 💻 Key DAX Measures
A sample of the custom Data Analysis Expressions (DAX) engineered for this project:

```dax
-- Total Revenue Calculation
Total Revenue = SUM(order_items[price])

-- Distinct Customer Count
Total Customers = DISTINCTCOUNT(customers[customer_id])

-- Average Freight Cost
Avg Shipping Cost = AVERAGE(order_items[freight_value])
---
```
## 📂 Project Structure

```text
olist-ecommerce-data-analysis/
│
├── 📂 data/
│   └── (Your CSV datasets here)
│
├── 📂 screenshots/
│   ├── overview.jpg
│   ├── products.jpg
│   └── customers.jpg
│
├── 📊 Olist_Ecommerce_Dashboard.pbix
├── 📑 Capstone_Presentation.pdf
├── 📜 README.md
└── ⚖️ LICENSE
---
```
## Clone the repository:
```git clone [https://github.com/](https://github.com/)[kuldeeprc2021-max]/Olist-Ecommerce-Data-Analysis.git```

## Author
**Kuldeep R. Choudhary**
* Microsoft Elevate AICTE Internship - Capstone Project
* Contact: [kuldeeprc2021@gmail.com]

## License
This project is licensed under the MIT License. 

```Analyzing Olist's e-commerce data is not just an academic exercise, it's about finding real strategic value in raw numbers.```
