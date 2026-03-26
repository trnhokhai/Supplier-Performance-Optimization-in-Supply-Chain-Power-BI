# Supplier Performance Analysis in Supply Chain | Power BI

![background](https://github.com/trnhokhai/Supplier-Performance-Optimization-in-Supply-Chain-Power-BI/blob/31e15f0fe4da50e70b04d54a4da81889d4f7077d/background.webp)
---

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



| # | Key Insight | Supporting Evidence | What This Means for the Business |
|---|------------|--------------------|---------------------------------|
| 1️⃣ | **Components Drive the Majority of Procurement Spend** | - Components account for **~$26M+** of total spend<br>- Accessories follow, Clothing is minimal<br>- Spend growth is mainly driven by Components | Procurement risk is heavily concentrated in Components. Any quality or supplier issue in this category would have significant financial and operational impact. |
| 2️⃣ | **Quality Risk Is Higher in High-Value Categories** | - Components reject rate: **~3.49%**<br>- Accessories reject rate: **~2.49%**<br>- Clothing has very low reject rate but low spend | The highest-spend category also carries the highest quality risk. Even small defect reductions in Components can deliver meaningful cost savings. |
| 3️⃣ | **Delivery Performance Is Consistent Across Categories** | - On-Time % near **100%** for Components and Accessories<br>- Lead time stable at **~9 days** | Delivery is not the primary issue at the category level. The bigger opportunity lies in reducing defect rates rather than improving speed. |
| 4️⃣ | **Cost Savings Do Not Clearly Offset Quality Risk** | - PPV% is relatively consistent across categories (**~5%**)<br>- No clear link between higher PPV and lower reject rates | Marginal price advantages should not outweigh quality considerations. Long-term efficiency depends more on defect reduction than small cost savings. |
| 5️⃣ | **Product-Level Variation Exists Within Strong Categories** | - Certain Component products show higher reject concentration<br>- Some high-spend products have slightly lower SRI | Category-level stability can hide product-level quality risk. Targeted product-level monitoring would improve control and risk management. |

**🎯 Executive Takeaway**

Procurement risk is not evenly distributed—it is concentrated in the **Components** category, which drives the majority of spend and carries higher reject rates.

The biggest improvement opportunity is to:

- Focus quality improvement efforts on high-spend categories  
- Monitor product-level defect concentration  
- Align spend growth with quality stability

## 🚀 Business Recommendations  

| # | Recommendation | Key Actions | Business Impact |
|---|----------------|-------------|-----------------|
| 1️⃣ | **Reallocate Spend Toward High-Quality Suppliers** | - Increase volume to suppliers with **reject rate < 3.12%** and **SRI ≥ 97%**<br>- Gradually reduce exposure to high-spend suppliers with reject rates **> 4–5%** | - Lower defect-related rework and inspection costs<br>- Improve operational stability<br>- Reduce quality-driven disruption risk |
| 2️⃣ | **Strengthen Quality Control in the Components Category** | - Set stricter reject thresholds for Components suppliers<br>- Conduct targeted reviews for high-reject vendors<br>- Monitor product-level defects within high-spend SKUs | - Reduce financial exposure in the highest-spend category<br>- Improve margin protection<br>- Prevent small quality issues from scaling |
| 3️⃣ | **Segment Suppliers by Performance Tier** | - Classify suppliers as **Strategic**, **Monitor**, or **At-Risk** based on SRI, reject rate, and spend exposure<br>- Use segmentation to guide contracts and volume allocation | - Clear vendor prioritization framework<br>- More structured sourcing decisions<br>- Better risk management |
| 4️⃣ | **Shift Focus from Delivery to Defect Reduction** | - Maintain current delivery standards (already near 100%)<br>- Redirect improvement efforts toward reducing reject rates | - Higher ROI from improvement initiatives<br>- Stronger long-term cost efficiency<br>- Improved supply chain reliability |
| 5️⃣ | **Monitor Performance During Spend Growth** | - Track SRI volatility during high PO periods<br>- Review supplier capacity before increasing volume | - Prevent performance breakdown during rapid scale<br>- Ensure sustainable procurement growth<br>- Maintain reliability while expanding operations |

## 🚀 Next Steps & Improvements

- **Quantify the financial impact of defects**  
  Convert reject rates into estimated costs of rework, returns, and production delays to better prioritize high-risk suppliers.

- **Develop a composite supplier score**  
  Combine quality, delivery, cost (PPV), and spend concentration into a single weighted score to enable clearer and more objective vendor ranking.

- **Implement a supplier tier dashboard**  
  Automatically classify suppliers into **Strategic**, **Monitor**, and **At-Risk** segments to support faster, data-driven decisions.

- **Add SKU-level risk monitoring**  
  Identify high-revenue or high-volume products with elevated reject rates to target quality improvement efforts more precisely.

- **Track supplier performance during growth periods**  
  Monitor SRI volatility when spend or PO volume increases to prevent performance degradation as the business scales.
