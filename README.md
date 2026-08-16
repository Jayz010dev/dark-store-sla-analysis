# Quick Commerce SLA Crisis: Finding the Real Cause Behind 85% Late Deliveries
### Dark Store Network Analysis Project | Python · Power BI

---

## The Business Problem

Quick commerce companies promise **10-minute delivery**. That's their entire value proposition.

But when we analyzed **1 million orders** across 12 Indian cities and 8 companies, we found something alarming:

> **84.88% of all orders are failing to meet the 10-minute SLA.**

That means nearly **9 out of every 10 deliveries** are arriving late. For an industry built on speed, this is an existential problem.

The question we set out to answer: **Why is this happening, and what needs to change?**

---

## What We Investigated

Most people assume late deliveries happen because stores are too far away. We tested that assumption and found it was wrong.

We investigated 3 possible causes:

| Cause | What We Found | Verdict |
|---|---|---|
| Dark store distance too far? | All companies average same distance (~7.75 km) | Ruled Out |
| Too many orders causing overload? | All cities handle same volume (~79,000 orders) | Ruled Out |
| Operational inefficiency? | Zepto: 9.57 min vs Jio Mart: 22.96 min, same distance | Root Cause |

---

## The Key Insight

**Zepto delivers in 9.57 minutes average. Jio Mart takes 22.96 minutes. Both travel the same distance.**

This single finding changes everything. The problem is not where dark stores are located — it is how fast companies process and dispatch orders once placed.

We confirmed this with a machine learning feature importance analysis:

| Factor | Contribution to SLA Breach |
|---|---|
| City Infrastructure | 46.8% |
| Company Operations | 37.0% |
| Delivery Distance | 16.2% |

**Distance — the thing everyone assumed was the problem — explains only 16% of breaches.**

---

## City-Level Discovery

Delhi stands out as a benchmark — only **16.4% breach rate** vs 88-100% in every other city, despite identical distances and order volumes.

| City | Breach Rate | Avg Delivery Time | Status |
|---|---|---|---|
| Delhi | 16.4% | 7.14 min | Good |
| Noida | 87.9% | 15.51 min | High |
| Mumbai | 93.6% | 17.51 min | Critical |
| Jaipur | 98.2% | 20.55 min | Critical |
| Haridwar | 100.0% | 27.54 min | Critical |

**Delhi's infrastructure and operational model is what every other city needs to replicate.**

---

## Company-Level Discovery

Even within the same city, companies perform very differently:

| Company | Breach Rate | Avg Delivery Time | Status |
|---|---|---|---|
| Zepto | 39.7% | 9.57 min | Good |
| Dunzo | 82.4% | 14.12 min | High |
| Blinkit | 87.8% | 15.07 min | High |
| Swiggy Instamart | 91.2% | 16.02 min | Critical |
| Big Basket | 93.5% | 17.98 min | Critical |
| Amazon Now | 94.3% | 18.94 min | Critical |
| Jio Mart | 98.0% | 22.96 min | Critical |

**Zepto is the only company consistently meeting the 10-min SLA — not because they are closer, but because they are faster at fulfillment.**

---

## The Hidden Problem Nobody Expected

Even orders delivered within **0-2 km** average **12.76 minutes** — already over SLA before distance is even a factor.

This means there is a fixed processing delay happening inside every dark store (picking, packing, dispatch) that no amount of store relocation will fix.

---

## Recommendations

**Priority 1 — Urgent**
- Audit Jio Mart operations immediately — 98% breach rate is unsustainable
- Add dark stores in Haridwar and Jaipur — 100% and 98% breach cities need immediate coverage

**Priority 2 — High**
- Reduce base processing time — mandate maximum 3-minute pick-pack-dispatch window
- Replicate Delhi's operational model in Mumbai, Bengaluru, and other critical cities
- Benchmark Zepto's fulfillment process and standardize across all companies

**Priority 3 — Medium**
- Introduce monthly SLA compliance reporting per company per city
- Introduce SLA penalty clauses for companies consistently above 85% breach rate

---

## Dashboard

4-page interactive Power BI dashboard covering:
- Page 1: Executive Summary — KPIs and breach rates by city and company
- Page 2: Root Cause Analysis — distance, delivery time, feature importance
- Page 3: City Deep Dive — interactive city filter and summary table
- Page 4: Recommendations — strategic actions and implementation priority

---

## Tools Used

Python, Pandas, NumPy, Scikit-learn, Jupyter Notebook, Power BI, Git, GitHub

---

## Author

**Jaydeep Jagdale**
Aspiring Data Analyst
LinkedIn: https://www.linkedin.com/in/jaydeep-jagdale-819b321b8
GitHub: https://github.com/Jayz010dev

---

## Dataset and Dashboard Links

- Cleaned Dataset: https://drive.google.com/file/d/1VjZkVoRw36xy9WCmXLMu0SWiK-9LT1mU/view?usp=drive_link
- Power BI Dashboard: https://drive.google.com/file/d/1sbvd2Y7RDsPnNECZG2iQP2mH0q9Ygziu/view?usp=drive_link
- Raw Dataset Source: https://www.kaggle.com/datasets/rohitgrewal/quick-commerce-dataset

---

*This project uses synthetic data inspired by real Indian quick commerce platforms. Created for educational and portfolio purposes.*
