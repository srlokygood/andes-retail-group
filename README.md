# 📊 Sales Performance & Diagnostic Analysis Dashboard (Power BI)

This repository contains a comprehensive **Business Intelligence & Data Analysis** project developed in Power BI. The primary objective is to evaluate the commercial performance of a retail business over a two-year period (2024–2025), diagnosing root causes behind revenue variations and delivering actionable strategic recommendations.

---

## 📌 Executive Summary & Context

Using a transactional dataset covering sales across **Peru, Chile, and Colombia**, an interactive analytics solution was designed with two distinct operational levels:
1. **Overview Dashboard:** Designed for executive decision-making (C-Suite / Management), providing a macro view of financial health, year-over-year (YoY) trends, and high-level business distribution.
2. **Diagnostic Detail View:** Built for deep exploratory analysis to identify the root causes of revenue fluctuations across seasons, customer segments, and product categories.

---

## 🖥️ Dashboard Architecture & Visual Walkthrough

### 1. Overview Dashboard (Vista General)

> *The Overview page is engineered to answer high-level executive questions: How is the business performing overall? Where are sales coming from? What is the trend across time?*

<!-- PLACEHOLDER FOR OVERVIEW IMAGE -->
![Overview Dashboard](<img width="1152" height="650" alt="image" src="https://github.com/user-attachments/assets/f8d2645d-1523-442f-b04b-fac323faecde" />)

#### 🔍 Explanation of Overview Components:
* **Executive KPI Cards:** Top-level indicators tracking **Total Revenue ($5.532M)**, **Total Cost ($3.590M)**, and **Units Sold (57.601K)** to establish immediate financial context[cite: 5].
* **Time-Series Revenue Trend (2024 vs. 2025):** Overlaid monthly line charts on a single 12-month axis[cite: 5]. This chart demonstrates that sales follow a highly predictable, cyclical seasonal curve across both years rather than suffering a structural annual collapse[cite: 5].
* **Geographic & Category Distribution:**
  * **By Country:** Identifies **Peru** as the top revenue contributor ($2.2M+), followed closely by **Chile** ($2.0M+) and **Colombia** ($1.3M+)[cite: 5].
  * **By Product Category:** Highlights **Sports** ($1.4M+) as the primary revenue engine, supported by Electronics, Home, and Clothing[cite: 5].
* **Customer Segment Breakdown:** Donut chart revealing high revenue concentration, where **Premium** ($2.598M / 46.97%) and **Standard** ($2.436M / 44.05%) customers generate **91.02% of total sales**, leaving Budget/Economic clients with only 8.98% ($497K)[cite: 5].

---

### 2. Diagnostic Detail View (Vista Detalle)

> *The Detail View enables root-cause exploration: Why did revenue drop during specific periods? Which customer segments and product verticals drove the contraction in 2025?*

<!-- PLACEHOLDER FOR DETAIL VIEW IMAGE -->
![Detail View Dashboard](<img width="1061" height="644" alt="image" src="https://github.com/user-attachments/assets/371653a9-b127-43d9-8c54-5b8f03525d8c" />)

#### 🔍 Explanation of Detail View Components:
* **Seasonal Comparison (`Ingresos Totales por temporada 2024 vs 2025`):** Line chart comparing cumulative revenue per season[cite: 8]. It proves that performance was virtually identical in Winter, Autumn, and Spring, isolating the YoY revenue gap entirely to the **Summer** season[cite: 8].
* **Monthly Segment Timeline (`Línea de tiempo de los ingresos totales por segmento de cliente`):** Multi-line timeline tracking monthly spend across customer tiers, highlighting key periods where Premium spending dipped below Standard accounts[cite: 8].
* **Interannual Segment Comparison (`Ingresos Totales por cada segmento de clientes 2024 vs 2025`):** Grouped bar chart showing that overall revenue contraction in 2025 was driven specifically by reduced spending in the **Premium** segment[cite: 8].
* **Interannual Category Comparison (`Ingresos totales de cada categoría 2024 vs 2025`):** Bar chart detailing the performance distribution across product lines (Sports, Electronics, Home, Clothing)[cite: 8].
* **Category x Customer Segment Cross-Analysis (`Ingresos totales de cada categoría por segmento de cliente`):**
  
  <!-- PLACEHOLDER FOR FILTERED DETAIL VIEW IMAGE -->
  ![Detail View Filtered 2025](<img width="265" height="203" alt="image" src="https://github.com/user-attachments/assets/87f6e8de-ddf4-407e-b962-978e74e31cff" />)

  * *Diagnostic Finding:* When filtering by **2025**, this chart exposes that the Premium segment's reduction in spend directly impacted **Home, Electronics, and Clothing**, while the **Sports** category remained resilient[cite: 8, 9].

---

## 🛠️ Methodology & Analytical Steps

To understand the business state and isolate underlying drivers, a 4-step framework was executed:

1. **Exploratory Phase & Metric Framing:** Defined core KPIs and structured business dimensions (*Country, Category, Customer Tier, Seasonality*)[cite: 5, 8].
2. **Iterative Design & UX Refinement:** Overlaid YoY time-series charts to disprove a structural business decline and confirm recurring seasonality[cite: 5].
3. **Root-Cause Diagnostics:** Leveraged cross-filtering in the Detail View to isolate 2025 revenue drops down to **Summer Season → Premium Clients → Home, Electronics & Clothing categories**[cite: 8, 9].
4. **Strategic SCQA Formulation:** Synthesized findings into executive-ready communication (Situation, Complication, Question, Answer)[cite: 5, 8].

---

## 💡 Key Business Insights & Next Steps

1. **Anti-Cyclical Summer Strategy (June – August):**
   * *Insight:* Revenue experiences a sharp ~70% drop mid-year during the summer slump[cite: 5, 8].
   * *Action:* Deploy targeted mid-year marketing campaigns, product bundles, and seasonal promotions to stabilize cash flow[cite: 5].
2. **Premium Client Retention Program:**
   * *Insight:* Premium clients drove the 2025 revenue decline by cutting back on Home, Electronics, and Clothing[cite: 8, 9].
   * *Action:* Implement personalized loyalty incentives, exclusive offers, and dedicated account outreach for high-value clients[cite: 8, 9].
3. **Cross-Selling via Sports Category:**
   * *Insight:* Sports is the only category where Premium customers maintained strong purchasing habits in 2025[cite: 8, 9].
   * *Action:* Use Sports products as an entry door to cross-sell items in Home and Electronics[cite: 8, 9].

---

## 🚀 Tools & Technologies

* **Power BI Desktop:** Data modeling, interactive visual design, and DAX measure development.
* **DAX (Data Analysis Expressions):** Time-intelligence calculations, YoY growth metrics, and conditional formatting.
* **Markdown & SCQA Framework:** Executive project documentation and asynchronous stakeholder reporting.
