# 🛒 Olist E-Commerce Sales & Performance Analytics

## 📌 Project Overview
This project is an end-to-end Business Intelligence dashboard built using **Microsoft Power BI**. It analyzes massive volumes of decentralized e-commerce data from Olist (a major Brazilian e-commerce platform) to provide executives and inventory managers with actionable, real-time insights into revenue tracking, product performance, and customer geographic distribution.

### 🛠️ Tools & Technologies Used
* **Microsoft Power BI:** Data modeling, DAX calculations, and interactive visualization.
* **Power Query Editor:** ETL (Extract, Transform, Load) processes and data cleaning.
* **Data Source:** Olist Brazilian E-commerce Public Dataset (Kaggle).

---

## 📊 The Dashboard 

### 1. Executive Overview
Designed for high-level stakeholders, this page tracks overarching KPIs against corporate targets and visualizes macro-level seasonal trends.
* **Key Features:** Target-tracking Gauge Chart, seasonal Revenue Trendline, and geographical sales density map.

![Overview Page](https://github.com/kuldeeprc2021-max/Olist-Ecommerce-Data-Analysis-Report-/blob/main/1774161719768.png)

### 2. Product Performance Deep-Dive
Built for inventory and supply chain managers to rapidly identify profitable items and dead stock.
* **Key Features:** Conditional Matrix formatting (Data Bars) for quick scanning, and dynamic Top 10 / Bottom 10 Revenue Generator bar charts.

![Products Page](https://github.com/kuldeeprc2021-max/Olist-Ecommerce-Data-Analysis-Report-/blob/main/1774161720433.png)

### 3. Customer & Geographic Insights
Tailored for marketing and logistics teams to understand regional customer density and acquisition trends.
* **Key Features:** Interactive bubble map of customer distribution, Treemap of top-performing cities, and month-over-month customer acquisition Area Chart.

![Customers Page](https://github.com/kuldeeprc2021-max/Olist-Ecommerce-Data-Analysis-Report-/blob/main/1774161721137.png)

---

## ⚙️ Methodology & System Approach

1. **Data Extraction & Transformation:** Ingested multiple raw CSV files (Orders, Customers, Products, Items). Handled null values, standardized currency formats, and engineered temporal features (Year/Month) using Power Query.
2. **Relational Data Modeling:** Architected a **Star Schema** to connect central fact tables (Orders) with dimension tables (Customers, Products), optimizing the VertiPaq engine for seamless cross-filtering.
3. **Analytical DAX Engineering:** Formulated custom DAX measures to calculate dynamic KPIs, including Distinct Customer Count, Total Revenue, and Average Shipping Cost.
4. **Interactive UI Deployment:** Developed a 3-page, app-like interface utilizing synced timeline slicers, custom navigation buttons, and advanced visual elements to ensure a highly intuitive user experience.

---

## 💡 Key Business Insights
* **Top Category:** `beleza_saude` (Health & Beauty) and `cama_mesa_banho` (Bed, Bath & Table) are the primary revenue drivers, making up a significant portion of total sales.
* **Regional Dominance:** The customer base is heavily concentrated in the São Paulo (SP) state, presenting opportunities for targeted regional marketing and localized distribution centers.
* **Underperforming Stock:** Specific niche categories like `pc_gamer` and `fashion_esporte` consistently rank in the bottom 10, indicating a need for inventory reduction or strategic marketing shifts.
