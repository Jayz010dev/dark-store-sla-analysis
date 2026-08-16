🚨 Quick Commerce SLA Crisis: Finding the Real Cause Behind 85% Late Deliveries
A Dark Store Network Analysis Project | Python · Power BI
---
🚨 The Business Problem
Quick commerce companies promise 10-minute delivery. That's their entire value proposition.
But when we analyzed 1 million orders across 12 Indian cities and 8 companies, we found something alarming:
> **84.88% of all orders are failing to meet the 10-minute SLA.**
That means nearly 9 out of every 10 deliveries are arriving late. For an industry built on speed, this is an existential problem.
The question we set out to answer: Why is this happening, and what needs to change?
---
🔎 What We Investigated
Most people assume late deliveries = stores are too far away. We tested that assumption — and found it was wrong.
We investigated 3 possible causes:
Cause	What We Found
Dark store distance too far?	❌ All companies average same distance (~7.75 km)
Too many orders (overload)?	❌ All cities handle same volume (~79,000 orders each)
Operational inefficiency?	✅ THIS is the real driver
---
💡 The Key Insight
Zepto delivers in 9.57 minutes average. Jio Mart takes 22.96 minutes. Both travel the same distance.
This single finding changes everything. The problem isn't where dark stores are located — it's how fast companies process and dispatch orders once they're placed.
We confirmed this with a machine learning feature importance analysis:
Factor	Contribution to SLA Breach
City infrastructure	46.8%
Company operations	37.0%
Delivery distance	16.2%
Distance — the thing everyone assumed was the problem — explains only 16% of breaches.
---
🏙️ City-Level Discovery
Delhi stands out as a benchmark — only 16.4% breach rate vs 88–100% in every other city, despite identical distances and order volumes.
City	Breach Rate	Avg Delivery Time
Delhi	16.4% ✅	7.14 min
Noida	87.9% ⚠️	15.51 min
Mumbai	93.6% 🔴	17.51 min
Jaipur	98.2% 🔴	20.55 min
Haridwar	100% 🔴	27.54 min
Delhi's infrastructure and operational model is what every other city needs to replicate.
---
📦 Company-Level Discovery
Even within the same city, companies perform very differently:
Company	Breach Rate	Avg Delivery Time
Zepto	39.7% ✅	9.57 min
Dunzo	82.4% ⚠️	14.12 min
Blinkit	87.8% ⚠️	15.07 min
Jio Mart	98.0% 🔴	22.96 min
Zepto is the only company consistently meeting the 10-min SLA — and it's not because they're closer. It's because they're faster at fulfillment.
---
⚠️ The Hidden Problem Nobody Expected
Even orders delivered within 0–2 km average 12.76 minutes — already over SLA before distance is even a factor.
This means there's a fixed delay happening inside the dark store (picking, packing, dispatch) that no amount of store relocation will fix.
---
✅ Recommendations
Priority 1 — Urgent
Audit Jio Mart operations immediately — 98% breach rate is unsustainable
Add dark stores in Haridwar & Jaipur — 100% and 98% breach rates, need immediate coverage
Priority 2 — High
Reduce base processing time — mandate max 3-min pick-pack-dispatch window
Replicate Delhi's operational model in Mumbai, Bengaluru, and other critical cities
Benchmark Zepto's fulfillment process and standardize across all companies
Priority 3 — Medium
Introduce monthly SLA compliance reporting per company per city
Introduce SLA penalty clauses for companies consistently above 85% breach rate
---
📊 Dashboard
4-page interactive Power BI dashboard covering:
Executive Summary (KPIs + breach rates)
Root Cause Analysis (distance, company, feature importance)
City Deep Dive (interactive slicer + summary table)
Recommendations (strategic actions + implementation priority)
---
🛠️ Tools Used
Python · Pandas · Scikit-learn · Jupyter Notebook · Power BI · Git
---
👤 Author [Jaydeep Jagdale]   
 Aspiring Data Analyst
 [www.linkedin.com/in/jaydeep-jagdale-819b321b8] | [Jayz010dev]
 ---
 Dataset: Synthetic quick commerce data (1M orders) inspired by Blinkit, Zepto, Swiggy Instamart, Jio Mart and other Indian platforms. For educational/portfolio    purposes.

## 📎 Dataset & Dashboard Links
- 📊 **Cleaned Dataset:** [https://drive.google.com/file/d/1VjZkVoRw36xy9WCmXLMu0SWiK-9LT1mU/view?usp=drive_link}
- 📈 **Power BI Dashboard:** [View on Google Drive](https://drive.google.com/file/d/1sbvd2Y7RDsPnNECZG2iQP2mH0q9Ygziu/view?usp=drive_link)

