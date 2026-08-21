# marketing-campaign-analytics

# 💄 Aura Beauty: Q2 Digital Marketing Analysis

![Domain](https://img.shields.io/badge/Domain-E--Commerce%20%26%20Marketing-brightgreen?style=for-the-badge)
![Power BI](https://img.shields.io/badge/Power_BI-Dashboard-yellow?style=for-the-badge)
![Excel](https://img.shields.io/badge/Excel-Modeling-darkgreen?style=for-the-badge)

---

## 📖 Project Overview

Aura Beauty is a fictional **Direct-to-Consumer (DTC)** skincare company operating in Kenya and investing heavily in digital advertising across **Meta, Google, and TikTok**.

This project analyzes the company's **Q2 marketing performance** by combining marketing analytics with unit economics to determine whether advertising spend is producing profitable customer growth.

Rather than relying on pre-calculated marketing metrics, every KPI is dynamically calculated from raw campaign data to ensure mathematical accuracy.

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

✔ Evaluate campaign performance across marketing channels.

✔ Calculate CTR, conversion rate, CPC, CPA and ROAS.

✔ Compare ad spend against revenue generated.

✔ Identify high- and low-performing campaigns.

✔ Analyze customer value using LTV.

✔ Develop reusable DAX measures in Power BI

✔ Compare performance across audiences, locations and campaign types.

✔ Develop an interactive Power BI dashboard.

✔ Prevent incorrect averaging of ratio metrics

✔ Recommend optimal Q3 budget allocation

---

# 🛠 Tools Used

| Tool | Purpose |
|-------|----------|
| **Excel** | Initial exploration & data cleaning |
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
| Ad_Spend | Marketing spend ($) |
| Revenue | Revenue generated ($) |
| LTV | Estimated customer lifetime value |

---

# 📖 Data Dictionary

| Column          | Description                | Type      |
| --------------- | -------------------------- | --------- |
| Campaign        | Campaign identifier/name   | Dimension |
| Date            | Campaign activity date     | Date      |
| Channel         | Marketing channel          | Dimension |
| Campaign Type   | Type of marketing campaign | Dimension |
| Target Audience | Intended customer segment  | Dimension |
| Location        | Geographic market          | Dimension |
| Language        | Campaign language          | Dimension |
| Impressions     | Number of ad views         | Measure   |
| Clicks          | Number of clicks           | Measure   |
| Conversions     | Number of conversions      | Measure   |
| Ad Spend        | Amount spent               | Measure   |
| Revenue         | Revenue generated          | Measure   |
| LTV             | Customer lifetime value    | Measure   |

---

# 📋 Sample Dataset

| Campaign | Channel | Impressions | Clicks | Conversions | Spend | Revenue | LTV |
|-----------|----------|------------:|-------:|------------:|------:|--------:|----:|
| CMP-000001 | Meta | 50,000 | 2,000 | 100 | $1,000 | $5,000 | $150 |
| CMP-000002 | Google | 20,000 | 1,500 | 150 | $1,200 | $9,000 | $150 |
| CMP-000003 | TikTok | 80,000 | 1,600 | 40 | $800 | $2,400 | $100 |

---

# ❓ Key Business Questions

This project will help investigate
**Channel performance**

Which channels generate the most impressions, clicks, conversions and revenue?

Which channels have the highest CTR?

Which channels have the highest conversion rate?

Which channels have the best ROAS?


**Campaign performance**

Which campaigns generate the most revenue?

Which campaigns have the highest ROAS?

Which campaigns have the lowest CPA?

Which campaigns are underperforming relative to their spend?


**Customer quality**

Which campaigns generate the highest LTV?

Does higher conversion volume correspond to higher customer value?

Which channels attract the most valuable customers?


**Audience & geography**

Which target audiences perform best?

Which locations generate the most revenue?

Are some audiences expensive to acquire but highly valuable?


**Budget allocation**

Where should additional marketing budget be allocated?

Which channels/campaign types should potentially receive less investment?


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




# 👤 Author

**Wangui Esther**

Aspiring Data Analyst | SQL | Power BI | Excel 

---
