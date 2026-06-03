# End-to-End Dynamic Sales Performance Dashboard (2020 - 2022)

## 📌 Project Overview
This project delivers an interactive, end-to-end Power BI business intelligence solution that transforms raw, unformatted Excel data into actionable operational insights. Monitoring **$16M in revenue across 113M orders**, the dashboard enables executives to audit sales performance across supervisors, product lines, brand market shares, and geographical regions in real time.

📊 **[Link to Live Interactive Dashboard (e.g., NovyPro/Power BI Service)](#)** *(Optional: Add link here)*

---

## 🛠️ Tech Stack & Skills Demonstrated
* **Business Intelligence:** Power BI Desktop / Power BI Service
* **ETL & Data Transformation:** Power Query, M Language
* **Data Modeling & Analytics:** DAX (Data Analysis Expressions), Relational Schemas
* **Data Source:** Microsoft Excel (Multi-sheet transaction logs)

---

## ⚙️ Architecture & Technical Implementation

### 1. Automated ETL Pipeline (Power Query)
To ensure the dashboard handles dynamic data refreshes flawlessly, a reusable automated data cleaning pipeline was built to fix common spreadsheet anomalies:
* **Schema Standardization:** Promoted headers, enforced strict data types (Currency, Integers, Dates), and removed blank rows/errors.
* **Text Normalization:** Trimmed leading/trailing whitespaces and standardized text casing across supervisor names and product categories.
* **Fact/Dim Splitting:** Parsed unpivoted transactional records into structured analytical tables.

### 2. Data Modeling & DAX Engineering
A clean star-schema design was implemented to maximize performance and cross-filtering efficiency. Core metrics were calculated using custom DAX formulas:

* **Total Sales:**
  ```dax
  Total Sales = SUM(Sales_Data[Sales_Amount])
  ```
* **Order Count:**
  ```dax
  Order Count = COUNTROWS(Sales_Data)
  ```
* **Total Cost:**
  ```dax
  Total Cost = SUM(Sales_Data[Cost_Amount])
  ```
* **Total Profit:**
  ```dax
  Total Profit = [Total Sales] - [Total Cost]
  ```

---

## 💡 Key Business Insights Captured

* **Product Demand Matrix:** Hardware items like **Monitors, CPUs, and Mice** dominate inventory throughput by quantity volume.
* **Market Share Concentration:** **Intel, Samsung, and Dell** constitute the core revenue drivers, representing a significant percentage of overall brand sales.
* **Geospatial Distribution:** The interactive map quickly isolates top-performing sales states to optimize regional supply chain allocation.

---

## 🚀 How to Run This Project Local
1. Clone this repository to your machine.
2. Open the `.pbix` file using **Power BI Desktop**.
3. *(Optional)* If modifying source data, update the file path parameters in Power Query to point to your local data file and click **Refresh**.

---

## 👤 Author
* **Name:** Diksha Jaykumar Rami
* **LinkedIn:** [Your LinkedIn Profile URL](#)
* **Portfolio:** [Your Portfolio URL/NovyPro](#)
