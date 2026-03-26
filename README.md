# Supplier Performance Analysis in Supply Chain | Power BI

![background](https://github.com/trnhokhai/Supplier-Performance-Optimization-in-Supply-Chain-Power-BI/blob/31e15f0fe4da50e70b04d54a4da81889d4f7077d/background.webp)
---

## Executive Summary

Supplier performance appears strong at a high level (97% SRI, ~100% On-Time), but deeper analysis reveals that risk is concentrated in a small group of high-spend suppliers and within the Components category, which accounts for the majority of procurement spend.

As procurement volume scales (+161% YoY), cost efficiency is deteriorating (PPV% ↑) while quality issues remain present, indicating early signs of scaling inefficiency.

A targeted approach—shifting volume away from high-risk suppliers, auditing defect-driving vendors, and diversifying sourcing in critical categories—can significantly reduce operational risk and improve procurement efficiency without broad structural changes.


## 📑 Table of Contents

- [📌 Background & Overview](#-background--overview)
- [📌 Data Source](#-data-source)
- [🧩 Data Modeling](#-data-modeling)
- [🧠 Design Thinking Process](#-design-thinking-process)
- [📊 Key Insights & Visualizations](#-key-insights--visualizations)
- [🚀 Business Recommendations](#-business-recommendations)
- [🔄 Next Steps & Improvements](#-next-steps--improvements)


## 📌 Background & Overview  

AdventureWorks is a bicycle manufacturing company that relies on a global supplier network for components and materials. As procurement spend increases, ensuring supplier performance becomes critical to maintaining product quality, delivery reliability, and cost control.

### Objective:
Evaluate supplier performance across delivery, quality, and cost to identify which suppliers to prioritize, where risks are concentrated, and how to scale procurement without increasing operational risk.


### 👤 Stakeholders

* Procurement Managers
* Supply Chain Managers
* Operations Leaders


### ❓ Key Business Questions

* Which suppliers should we prioritize as spend increases?
* Are we over-dependent on a small group of suppliers?
* Where is quality risk concentrated?
* Are cost changes (PPV%) aligned with performance?
* How can we scale procurement without increasing risk?

---

## 📌 Data Source

- **Source:** Kaggle – AdventureWorks Dataset  
- **Size:** The `Purchase_OrderDetails` table contains **8,845 records**  
- **Format:** PBIX

## Data Modeling

<img width="1216" height="721" alt="image" src="https://github.com/user-attachments/assets/9a5b9707-f565-48b7-ac3d-b17cf3142a58" />

## 🧠 Design Thinking Process  
1️⃣ Empathize

2️⃣ Define point of view

3️⃣ Ideate

4️⃣ Prototype and review

## 📊 Key Insights & Visualizations
### 🔍 Overview


<img width="1426" height="795" alt="image" src="https://github.com/user-attachments/assets/dcf0e4fc-bf8f-4210-aefc-a07f312e2175" />


#### 📊 Key Insights - Overview

| Insight | Details |
|--------|--------|
| Overall performance is strong, but not fully stable | SRI (97.3%) and On-Time (99.9%) are high, but reliability fluctuates over time, especially as volume increases |
| Rapid spend growth increases exposure to supplier risk | Spend grew +161% YoY, significantly increasing dependency on suppliers and amplifying the impact of any performance issues |
| Cost efficiency is deteriorating as procurement scales | PPV% has increased, indicating rising costs despite stable delivery performance |
| Quality is improving, but remains inconsistent | Reject rate decreased, but past volatility suggests quality is not fully under control |
| Spend concentration creates category and supplier dependency risk | ~77% of spend is in Components, with a large share concentrated among top suppliers |
| Lower-rated suppliers show improvement but may still pose risk | Higher SRI improvement among lower credit suppliers suggests recovery, but also indicates prior performance issues |

---

### 🤝 Supplier

<img width="1427" height="792" alt="image" src="https://github.com/user-attachments/assets/8f1da7df-032b-440f-9849-ce316242f351" />


#### 📊 Key Insights - Supplier

| Insight | Details |
|--------|--------|
| Spend is highly concentrated, increasing dependency risk | 80% of total spend is concentrated in just 24 suppliers, creating significant exposure if performance issues occur within this group |
| High-spend suppliers are not consistently high-performing | Several high-spend suppliers show elevated reject rates (e.g., Superior Bicycles), indicating that critical suppliers are also key sources of quality risk |
| Supplier risk is not evenly distributed, but concentrated in a few vendors | The supplier risk matrix shows that most suppliers perform within acceptable ranges, while a small group falls into high-risk zones (high spend + high reject) |
| Some suppliers show worsening quality trends despite stable overall metrics | Reject YoY highlights specific suppliers with increasing defect rates, signaling early-stage performance deterioration that may not yet impact overall KPIs |
| Top suppliers maintain high delivery performance but create over-dependence risk | While top suppliers show strong SRI and On-Time performance, reliance on a limited number of vendors reduces supply chain resilience |
| Supplier performance varies within the same credit tier | Even within “Excellent Credit” suppliers, performance varies in reject rate and PPV, indicating that credit rating alone is not sufficient for supplier evaluation |

---

#### Product 

<img width="1427" height="797" alt="image" src="https://github.com/user-attachments/assets/9e2c58f3-7563-4c8a-8286-39ad58f757ce" />

#### 📊 Key Insights


| Insight | Details |
|--------|--------|
| Spend is heavily concentrated in Components, driving overall risk exposure | Components account for ~77% of total spend, making this category the primary source of procurement risk |
| Higher spend categories also show higher quality risk | Components have a higher reject rate, indicating that the largest spend area is also the most vulnerable |
| Higher-value products amplify the impact of defects | Products with higher spend tend to have higher reject rates, increasing the financial impact of quality issues |
| Risk is concentrated in specific subcategories rather than evenly distributed | A small number of subcategories drive most of the quality issues, suggesting targeted improvement opportunities |

---

## 🚀 Business Recommendations & Impacts

| Recommendation | Action | Business Impact |
|---------------|--------|-----------------|
| Reallocate volume away from high-risk suppliers | Reduce 10–20% volume from high-spend, high-reject suppliers (e.g., Superior Bicycles) and shift to higher-performing alternatives | Reduces defect exposure and minimizes operational disruption from critical suppliers |
| Initiate immediate audit for top defect-driving suppliers | Prioritize the top suppliers contributing the highest reject rates for quality audits and corrective action plans | Addresses root causes of defects and prevents recurring quality issues at scale |
| Secure long-term agreements with high-performing suppliers | Increase commitment to suppliers with high SRI and low reject rates through contracts or preferred supplier status | Stabilizes supply and ensures reliable performance as procurement volume grows |
| Diversify sourcing within high-spend categories (Components) | Introduce additional qualified suppliers to reduce reliance on a small group of vendors | Improves supply chain resilience and reduces dependency risk in critical categories |
| Reassess suppliers with rising PPV% before further scaling | Evaluate whether cost increases are justified by performance; limit expansion with suppliers showing both rising cost and quality issues | Prevents cost escalation without corresponding value improvement |

--- 

## 🚀 Next Steps & Improvements


* **Incorporate supplier capacity and contract data**
  Analyze supplier capacity limits and contract terms to better support sourcing and allocation decisions.

* **Track supplier performance over shorter time intervals**
  Move from annual to monthly/quarterly analysis to detect performance issues earlier.

* **Include root cause data for defects and delays**
  Integrate defect types or return reasons to identify specific drivers of quality issues.

* **Expand cost analysis beyond PPV%**
  Include total cost factors such as transportation, rework, and inventory holding to better evaluate supplier value.

* **Develop a supplier scorecard for ongoing monitoring**
  Standardize key metrics (cost, quality, delivery) into a consistent evaluation framework for continuous tracking.

