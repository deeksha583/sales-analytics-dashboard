# sales-analytics-dashboard
"Interactive sales analytics dashboard for FY 2023 — built with HTML, CSS &amp; Chart.js. Visualizes revenue trends, channel performance, regional breakdown, top products, warehouse efficiency, and customer spend. Single-file, zero dependencies, deployable via GitHub Pages."

# 📊 Sales Analytics Dashboard

![GitHub Pages](https://img.shields.io/badge/Live-GitHub%20Pages-blue?style=flat-square&logo=github)
![Chart.js](https://img.shields.io/badge/Chart.js-4.4.1-FF6384?style=flat-square&logo=chartdotjs)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

> An interactive, client-side sales analytics dashboard built with HTML, CSS & Chart.js — visualizing FY 2023 sales performance across channels, regions, products, and warehouses.

---

## 🌐 Live Preview

**👉 [Click here to open the live dashboard](https://deeksha583.github.io/sales-analytics-dashboard/)**

---

## 📸 Dashboard Preview

![Full Dashboard Preview](https://raw.githubusercontent.com/deeksha583/sales-analytics-dashboard/main/assets/screenshots/dashboard-preview.png)

![Charts Section](https://raw.githubusercontent.com/deeksha583/sales-analytics-dashboard/main/assets/screenshots/charts-preview.png)

---

## 🗂️ Table of Contents

- [Overview](#overview)
- [Objectives](#objectives)
- [Data](#data)
- [Variables](#variables)
- [Methodology](#methodology)
- [Tools & Techniques](#tools--techniques)
- [Key Insights](#key-insights)
- [Project Files](#-project-files)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Conclusion](#conclusion)

---

## Overview

The **Sales Analytics Dashboard** is a fully self-contained, single-file web application that provides a comprehensive view of a company's sales performance for FY 2023. It renders multiple interactive charts covering revenue trends, channel distribution, regional breakdown, product performance, warehouse efficiency, and customer spend — all without any backend or build process required.

---

## Objectives

1. Consolidate key sales metrics into a single, accessible interface.
2. Visualize monthly revenue and order volume trends over 12 months.
3. Compare sales performance across channels — Online, Wholesale, Distributor, Export.
4. Identify top-performing products, regions, and customers.
5. Evaluate warehouse fulfillment efficiency across all locations.
6. Support data-driven decisions through actionable quick-prompt buttons.

---

## Data

| Attribute       | Details                                        |
|-----------------|------------------------------------------------|
| **Source**      | Simulated FY 2023 internal sales records       |
| **Time Period** | January 2023 – December 2023 (12 months)       |
| **Scope**       | All channels · All warehouses · All regions    |
| **Format**      | JavaScript arrays embedded in HTML             |
| **Orders**      | 3,847 total orders across 924 unique customers |

### Monthly Revenue & Orders

| Month | Revenue ($K) | Orders |
|-------|-------------|--------|
| Jan   | 298         | 241    |
| Feb   | 312         | 258    |
| Mar   | 345         | 289    |
| Apr   | 389         | 312    |
| May   | 401         | 334    |
| Jun   | 378         | 301    |
| Jul   | 415         | 348    |
| Aug   | 442         | 371    |
| Sep   | 398         | 322    |
| Oct   | 467         | 389    |
| Nov   | 512         | 421    |
| Dec   | 465         | 361    |
| **Total** | **$4,822K** | **3,847** |

### Sales by Channel

| Channel     | Share (%) | Est. Revenue |
|-------------|-----------|--------------|
| Online      | 38%       | ~$1,832K     |
| Wholesale   | 29%       | ~$1,398K     |
| Distributor | 21%       | ~$1,013K     |
| Export      | 12%       | ~$579K       |

### Sales by Region

| Region        | Revenue     |
|---------------|-------------|
| North America | $1,842,000  |
| Europe        | $1,231,000  |
| Asia-Pacific  | $897,000    |
| Latin America | $512,000    |
| Middle East   | $338,000    |

### Top 8 Products by Revenue

| Rank | Product       | Revenue |
|------|---------------|---------|
| 1    | Widget Pro    | $624K   |
| 2    | SolarPanel X2 | $589K   |
| 3    | DataSync Hub  | $512K   |
| 4    | EcoBottle Set | $478K   |
| 5    | ThermoKit     | $421K   |
| 6    | SmartSeal     | $389K   |
| 7    | PowerPack     | $356K   |
| 8    | AirFilter+    | $312K   |

### Warehouse Fulfillment Time

| Warehouse | Avg Days | Status   |
|-----------|----------|----------|
| WH-01     | 1.8 days | ✅ Fast  |
| WH-02     | 2.1 days | ✅ Fast  |
| WH-03     | 2.4 days | ⚠️ Avg  |
| WH-04     | 3.2 days | ⚠️ Slow |
| WH-05     | 3.9 days | ❌ Slow  |

---

## Variables

### KPI Summary

| Variable         | Value    | Change          |
|------------------|----------|-----------------|
| Total Sales      | $4.82M   | +12.4% YoY      |
| Total Orders     | 3,847    | +8.1% YoY       |
| Avg Unit Price   | $68.40   | Across all SKUs |
| Gross Margin     | 38.2%    | +2.1pp YoY      |
| Unique Customers | 924      | +63 new         |
| Avg Ship Delay   | 2.3 days | −0.4d improved  |

### JavaScript Variables (in index.html)

```javascript
const months  = ['Jan','Feb','Mar','Apr','May','Jun','Jul','Aug','Sep','Oct','Nov','Dec'];
const revenue = [298, 312, 345, 389, 401, 378, 415, 442, 398, 467, 512, 465];
const orders  = [241, 258, 289, 312, 334, 301, 348, 371, 322, 389, 421, 361];
```

---

## Methodology

1. **Data Structuring** — Sales data organized into flat JavaScript arrays.
2. **KPI Derivation** — Summary metrics pre-aggregated as static display values.
3. **Visual Encoding** — Each dimension mapped to the most appropriate chart type.
4. **Dual-Axis Design** — Monthly trend uses dual Y-axis to overlay revenue and orders.
5. **Color Coding** — Consistent 5-color palette across all charts:
   - `#378ADD` Blue · `#1D9E75` Green · `#EF9F27` Amber · `#D4537E` Rose · `#7F77DD` Violet
6. **Conditional Colors** — Warehouse bars: green (fast) / amber (avg) / red (slow).

---

## Tools & Techniques

| Tool           | Version | Purpose                          |
|----------------|---------|----------------------------------|
| HTML5          | —       | Structure and layout             |
| CSS3           | —       | Styling, grid, responsive design |
| JavaScript ES6 | —       | Data binding, chart logic        |
| Chart.js       | 4.4.1   | All 8 interactive charts         |
| CSS Variables  | —       | Theming and dark mode            |
| CSS Grid       | —       | Responsive card layout           |
| ARIA Labels    | —       | Screen reader accessibility      |

**Chart types used:** Line (dual axis) · Doughnut · Horizontal Bar · Bubble · Pie · Bar

---

## Key Insights

- 📈 **Revenue peaked in November** at $512K — strong Q4 seasonality.
- 🛒 **Online is the top channel** at 38% (~$1.83M).
- 🌍 **North America leads** at $1.84M (38% of total).
- 🏆 **Widget Pro** is the top product at $624K.
- 💰 **Higher price = better margin** — products above $150 show 47–52% margins.
- 🏭 **WH-01 fastest** at 1.8 days; **WH-05 needs improvement** at 3.9 days.
- 👤 **Top 6 customers** account for ~$1.4M (29% of total revenue).
- 💵 **USD dominates** at 52% of order value.

---

## 📁 Project Files

| File | Type | Link |
|------|------|------|
| 🌐 Live Dashboard | Web App | [**Open Live**](https://deeksha583.github.io/sales-analytics-dashboard/) |
| 📄 index.html | Source Code | [View Code](https://github.com/deeksha583/sales-analytics-dashboard/blob/main/index.html) |
| 📘 README.md | Documentation | [View README](https://github.com/deeksha583/sales-analytics-dashboard/blob/main/README.md) |
| 📊 Monthly Revenue | CSV | [Download](https://github.com/deeksha583/sales-analytics-dashboard/raw/main/assets/data/monthly_revenue.csv) |
| 📊 Products | CSV | [Download](https://github.com/deeksha583/sales-analytics-dashboard/raw/main/assets/data/products.csv) |
| 📊 Sales by Channel | CSV | [Download](https://github.com/deeksha583/sales-analytics-dashboard/raw/main/assets/data/sales_by_channel.csv) |
| 📊 Sales by Region | CSV | [Download](https://github.com/deeksha583/sales-analytics-dashboard/raw/main/assets/data/sales_by_region.csv) |
| 📊 Warehouse Fulfillment | CSV | [Download](https://github.com/deeksha583/sales-analytics-dashboard/raw/main/assets/data/warehouse_fulfillment.csv) |
| 📊 Top Customers | CSV | [Download](https://github.com/deeksha583/sales-analytics-dashboard/raw/main/assets/data/top_customers.csv) |
| 📊 Currency Split | CSV | [Download](https://github.com/deeksha583/sales-analytics-dashboard/raw/main/assets/data/currency_split.csv) |

---

## Project Structure

```
sales-analytics-dashboard/
│
├── index.html                     ← Main dashboard (single-file app)
├── README.md                      ← This file
│
├── assets/
│   ├── screenshots/
│   │   ├── dashboard-preview.png  ← Full dashboard screenshot
│   │   └── charts-preview.png     ← Charts section screenshot
│   └── data/
│       ├── monthly_revenue.csv
│       ├── products.csv
│       ├── sales_by_channel.csv
│       ├── sales_by_region.csv
│       ├── warehouse_fulfillment.csv
│       ├── top_customers.csv
│       └── currency_split.csv
```

---

## Getting Started

### Run Locally

```bash
git clone https://github.com/deeksha583/sales-analytics-dashboard.git
cd sales-analytics-dashboard
open index.html
```

### Live on GitHub Pages

🔗 **[https://deeksha583.github.io/sales-analytics-dashboard/](https://deeksha583.github.io/sales-analytics-dashboard/)**

To enable: **Settings → Pages → Source: main / root → Save**

---

## Conclusion

This dashboard delivers executive-level sales intelligence in a zero-dependency, single-file format — visualizing $4.82M in FY 2023 revenue across 8 chart types, 4 channels, 5 regions, 8 products, 5 warehouses, and 924 customers.

**Planned improvements:**
- [ ] CSV file upload for live data
- [ ] Date range picker
- [ ] Export to PDF / PNG
- [ ] Dark mode toggle
- [ ] Drill-down views per channel

---

*Built by [deeksha583](https://github.com/deeksha583) · HTML · CSS · JavaScript · Chart.js 4.4.1*
