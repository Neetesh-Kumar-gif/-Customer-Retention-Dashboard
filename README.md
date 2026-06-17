# 📊 Customer Retention Dashboard | Jan–Jun 2025
> End-to-end analytics project built with **Python** and **Power BI** to analyze customer retention, cohort behavior, and revenue trends for an Ayurvedic & Unani healthcare brand.

---

## 🧠 Business Problem

The business needed to understand:
- Are new customers coming back after their first purchase?
- Which months and products drive the most revenue?
- Is retention improving, declining, or staying flat across cohorts?

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **Python (Pandas)** | Data cleaning, cohort engineering, feature generation |
| **Power BI** | Dashboard design, DAX measures, multi-page reporting |
| **DAX** | Custom KPIs — Retention %, NTB Count, Revenue aggregations |

---

## 📁 Project Structure

```
customer-retention-dashboard/
│
├── data/
│   ├── raw/                  # Original transaction data
│   └── processed/            # Cohort-enriched output from Python
│
├── python/
│   └── cohort_analysis.py    # Cohort generation & data prep script
│
├── powerbi/
│   └── retention_dashboard.pbix  # Power BI report file
│
└── README.md
```

---

## 📐 Python — What It Does

- Parses raw order-level transaction data
- Assigns each customer their **first purchase month** (cohort)
- Calculates **month offset** (how many months since first purchase)
- Outputs two clean tables:
  - `cohort_enriched` — order-level data with cohort tags
  - `cohort_matrix` — pivot of retention % by cohort × month offset

---

## 📊 Power BI — Dashboard Pages

### Page 1: Executive Overview
- **KPI Cards** — Total Revenue (₹49.3M), Total Orders (35.2K), NTB Customers (8.6K), Returning Customers (7.4K)
- **Monthly Revenue Trend** — Line chart showing ₹6.1M → ₹10.1M growth (64% in 6 months)
- **New vs Returning Customers by Month** — Stacked bar chart with NTB & returning breakdown
- **Revenue by Product** — Horizontal bar chart; Immunity Booster leads at ₹10.1M
- **Total Revenue by Category** — Donut chart; Ayurvedic (60.28%) vs Unani (39.72%)
- **Category Filter** — Slicer to toggle between Ayurvedic and Unani views

### Page 2: Cohort Retention Matrix
- **KPI Cards** — Avg Retention (69.03%), Total NTB Count (29.7K), Total Returners (20.5K)
- **Cohort Matrix Table** — Retention % by cohort month × month offset, with conditional arrow icons
- **NTB Customers per Month** — Bar chart showing new customer acquisition trend
- **Retention Trend by Cohort** — Line chart comparing retention trajectories across cohorts
- **Business Interpretation Panel** — Key written insights embedded directly in the report

---

## 📈 Key Findings

| Insight | Detail |
|--------|--------|
| 🔁 Avg Retention | **69.03%** — ~7 in 10 new customers return |
| 📦 Top Product | **Immunity Booster** — ₹10.1M revenue |
| 🌿 Top Category | **Ayurvedic** — 60.28% of total revenue |
| 📅 Best Cohort | **January 2025** — retained 67–70% across 5 months |
| 📊 Revenue Growth | **₹6.1M → ₹10.1M** in 6 months (+64%) |
| 🔄 Retention Pattern | Consistent 65–72% across all cohorts — **product-driven, not seasonal** |

---

## 💡 Business Interpretation (from Report)

> *"January batch had 3,550 new customers. 67% returned in February, 70% in March, and this stayed consistent through June — 7 out of 10 new customers are becoming repeat buyers."*

> *"Regardless of which month customers first bought from us — January, February, March — they all retain at similar rates of 65–72%. This means our retention is consistent and product-driven, not seasonal."*

---


---


---

