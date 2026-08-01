# marketing-campaign-analytics

# 💄 Aura Beauty: Q2 Digital Marketing Analysis

![Domain](https://img.shields.io/badge/Domain-E--Commerce%20%26%20Marketing-brightgreen?style=for-the-badge)
![SQL](https://img.shields.io/badge/SQL-Analytics-blue?style=for-the-badge)
![Power BI](https://img.shields.io/badge/Power_BI-Dashboard-yellow?style=for-the-badge)
![Excel](https://img.shields.io/badge/Excel-Modeling-darkgreen?style=for-the-badge)

---

## 📖 Project Overview

Aura Beauty is a fictional **Direct-to-Consumer (DTC)** skincare company operating in Kenya and investing heavily in digital advertising across **Meta, Google, and TikTok**.

This project analyzes the company's **Q2 marketing performance** by combining marketing analytics with unit economics to determine whether advertising spend is producing profitable customer growth.

Rather than relying on pre-calculated marketing metrics, every KPI is dynamically calculated from raw campaign data to ensure mathematical accuracy.

---

# 📌 Executive Summary

The objective of this analysis is to evaluate the effectiveness of Aura Beauty's paid marketing strategy using industry-standard acquisition metrics such as:

- Customer Acquisition Cost (CAC)
- Return on Ad Spend (ROAS)
- Customer Lifetime Value (LTV)
- LTV:CAC Ratio
- Click Through Rate (CTR)
- Cost Per Click (CPC)

The final recommendations focus on how the marketing team should redistribute advertising budget for **Q3** to maximize long-term profitability rather than simply increasing traffic.

---

# 🎯 Business Problem

As Aura Beauty expands its digital marketing investment, management lacks visibility into three critical areas.

### 1️⃣ Channel Efficiency

Which advertising platform delivers the strongest return?

- Highest ROAS
- Lowest CAC
- Highest conversion efficiency

---

### 2️⃣ Customer Quality

Does a platform generating high traffic also generate valuable long-term customers?

In particular:

- Is TikTok producing quality customers?
- Does Meta outperform Google in lifetime value?
- Which channel provides the highest LTV:CAC ratio?

---

### 3️⃣ Data Accuracy

Executive reports currently average campaign ratios (CTR, CPC, Conversion Rate), producing misleading portfolio-level KPIs.

This project rebuilds all calculations using proper weighted aggregation.

---

# 🚀 Project Objectives

✔ Build robust SQL models from raw campaign data

✔ Develop reusable DAX measures in Power BI

✔ Prevent incorrect averaging of ratio metrics

✔ Validate all calculations against benchmark values

✔ Recommend optimal Q3 budget allocation

---

# 🛠 Tools Used

| Tool | Purpose |
|-------|----------|
| **Excel** | Initial exploration & data cleaning |
| **SQL** | Data transformation and KPI calculations |
| **Power BI** | Dashboard creation & executive reporting |
| **DAX** | Dynamic marketing metrics |
| **GitHub** | Documentation & project portfolio |

---

# 📂 Dataset Overview

The dataset contains campaign-level advertising performance across major Kenyan cities.

Derived marketing metrics were intentionally removed so they could be calculated dynamically.

## Raw Variables

| Column | Description |
|---------|-------------|
| Campaign_ID | Unique campaign identifier |
| Date | Campaign date |
| Channel | Meta, Google, TikTok |
| Campaign_Type | Prospecting, Search, Retargeting |
| Location | Nairobi, Mombasa |
| Impressions | Number of ad views |
| Clicks | Number of clicks |
| Conversions | Purchases generated |
| Ad Spend | Marketing spend ($) |
| Revenue | Revenue generated ($) |
| LTV | Estimated customer lifetime value |

---

# 📋 Sample Dataset

| Campaign | Channel | Impressions | Clicks | Conversions | Spend | Revenue | LTV |
|-----------|----------|------------:|-------:|------------:|------:|--------:|----:|
| CMP-001 | Meta | 50,000 | 2,000 | 100 | $1,000 | $5,000 | $150 |
| CMP-002 | Google | 20,000 | 1,500 | 150 | $1,200 | $9,000 | $150 |
| CMP-003 | TikTok | 80,000 | 1,600 | 40 | $800 | $2,400 | $100 |

---

# ❓ Key Business Questions

This project answers questions such as:

- Which channel has the highest ROAS?
- Which platform acquires customers at the lowest cost?
- Does TikTok's large reach generate profitable customers?
- Which platform has the strongest LTV:CAC ratio?
- Which campaigns should receive additional funding?
- Which campaigns should be paused?
- How should Aura Beauty allocate its Q3 marketing budget?

---

# 📐 KPI Definitions

| Metric | Formula |
|---------|---------|
| CTR | Clicks ÷ Impressions |
| CPC | Ad Spend ÷ Clicks |
| Conversion Rate | Conversions ÷ Clicks |
| CAC | Ad Spend ÷ Conversions |
| ROAS | Revenue ÷ Ad Spend |
| LTV:CAC | LTV ÷ CAC |

---

# 🧮 Validation Rules

To avoid misleading executive reports, every KPI is calculated from **aggregated base values**, not averages of campaign-level ratios.

### Correct Formulas

```
CTR  = Σ Clicks / Σ Impressions

CPC  = Σ Ad Spend / Σ Clicks

CAC  = Σ Ad Spend / Σ Conversions

ROAS = Σ Revenue / Σ Ad Spend

LTV:CAC = LTV / CAC
```

---

# ✅ Ground Truth Validation

### Campaign-Level Validation

| Metric | Expected |
|---------|---------:|
| CTR | 4.00% |
| CPC | $0.50 |
| Conversion Rate | 5.00% |
| ROAS | 5.00x |
| CAC | $10.00 |
| LTV:CAC | 15.0x |

---

### Portfolio-Level Validation

| KPI | Correct Value |
|------|--------------:|
| Portfolio CTR | **3.40%** |
| Conversion Rate | **5.69%** |
| CPC | **$0.59** |
| ROAS | **5.47x** |
| CAC | **$10.34** |

---

# 📊 Deliverables

- ✔ SQL scripts
- ✔ Data cleaning workflow
- ✔ Power BI dashboard
- ✔ DAX calculations
- ✔ Business insights
- ✔ Executive recommendations

---

# 📈 Expected Insights

After completing this project, stakeholders will understand:

- Which marketing channel deserves more investment
- Which campaigns destroy profitability
- Which customer acquisition strategy scales best
- How to improve marketing ROI in Q3
- How to correctly calculate portfolio marketing KPIs






# 👤 Author

**Esther Wangui Chege**

Aspiring Data Analyst | SQL | Power BI | Excel | Python

---
