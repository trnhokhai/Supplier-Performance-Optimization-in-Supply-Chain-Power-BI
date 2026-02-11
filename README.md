# Supplier Performance Optimization in Supply Chain | Power BI

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
### Objective: To evaluate supplier performance based on delivery reliability, product quality, and cost efficiency in order to prioritize vendors and reduce operational risk.
### 📖 What is this project about?

This project analyzes supplier performance using real procurement data from **AdventureWorks**.

As purchasing volume grows, companies need to ensure their suppliers can keep up—without causing delays, defects, or hidden costs.

Through this dashboard, I examined:

- Who delivers on time consistently  
- Which suppliers have higher defect rates  
- Where procurement spend is concentrated  
- Whether cost savings come with quality trade-offs  

The goal is to turn supplier data into clear, practical actions that help the business allocate spend more wisely.

### 👤 Who is this project for?  

- Procurement Managers  
- Supply Chain Managers  
- Operations Leaders  

It helps them decide:

- Which suppliers deserve more volume  
- Which suppliers require closer monitoring  
- Where quality risk is concentrated  
- How to scale purchasing without increasing risk

### Business Question ?

- Which suppliers should we prioritize as spend increases?  
- Are we over-dependent on certain vendors?  
- Where is quality risk concentrated?  
- Are cost savings worth the potential defect risk?  
- How can we grow procurement volume without hurting reliability?

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
### 🔍 Dashboard Preview
#### 📋 Executive Summary

<img width="1452" height="818" alt="image" src="https://github.com/user-attachments/assets/754df06a-9c0f-4b21-b983-9b5bd009ed58" />

| # | Key Insight | Supporting Evidence | What This Means for the Business |
|---|------------|--------------------|---------------------------------|
| 1️⃣ | **Overall Supplier Reliability Is Strong and Stable** | - Supplier Reliability Index (SRI): **97.3%**, slightly improving YoY<br>- On-Time Delivery: **99.92%**<br>- Reject Rate improved from **4.7% → 3.12%** | The supplier base is operationally stable. Delivery performance is not the main issue, and quality control has strengthened over time. |
| 2️⃣ | **Spend Has Grown Rapidly — Risk Must Be Managed** | - Total procurement spend increased from **$24.4M → $63.8M (+161%)**<br>- Performance metrics improved only marginally | The company is scaling fast. As volume grows, supplier risk exposure increases. Strong performance today does not guarantee stability under future growth. |
| 3️⃣ | **Performance Dip During High Volume Periods** | - SRI dropped in early **2013** when PO volume spiked<br>- Performance later stabilized above **97%** | Rapid increases in purchasing volume can stress suppliers. Performance should be closely monitored during growth phases to prevent breakdowns. |
| 4️⃣ | **Spend Is Highly Concentrated in Components** | - Components account for the majority of procurement spend<br>- Accessories and Clothing represent much smaller shares | Risk is concentrated in a single major category. Any disruption or quality issue in Components would have a significant financial impact. |
| 5️⃣ | **Quality Is the Real Differentiator — Not Delivery** | - On-Time % remains consistently high across suppliers<br>- Reject % varies noticeably over time | Delivery performance is under control. The biggest opportunity lies in reducing defect rates, especially in high-spend categories. |
| 6️⃣ | **High- Spend Vendors Are Not Always the Best Performers** | - Some high-spend suppliers have similar or lower SRI than mid-tier vendors<br>- Spend allocation does not fully align with performance | There is an opportunity to reallocate volume toward higher-performing suppliers to reduce operational and quality risk. |

**🎯 Executive Takeaway**

The supplier network is reliable and scalable, but rapid spend growth and category concentration increase exposure to quality risk.

The primary opportunity is not improving delivery speed—it is reducing defects and optimizing spend allocation toward high-performing suppliers.

#### 🤝 Supplier

<img width="1453" height="813" alt="image" src="https://github.com/user-attachments/assets/b9316af2-e837-46f7-a66a-be56216a93eb" />

| # | Key Insight | Supporting Evidence | What This Means for the Business |
|---|------------|--------------------|---------------------------------|
| 1️⃣ | **Spend Is Concentrated Among a Small Group of Suppliers** | - **24** active suppliers<br>- A small subset accounts for the majority of spend<br>- Top supplier represents **$4M+** in procurement volume | The company is moderately dependent on a few key suppliers. Any performance decline or disruption would have a significant operational impact. |
| 2️⃣ | **Quality Varies More Than Delivery** | - On-Time % near **100%** across suppliers<br>- Actual Lead Time stable at ~**9 days**<br>- Reject % varies widely (some **>5%**) | Delivery reliability is under control. Supplier differentiation comes mainly from quality performance, making defect reduction the top priority. |
| 3️⃣ | **High Spend Does Not Always Mean High Performance** | - Some high-spend suppliers have reject rates above the portfolio average (**3.12%**)<br>- Mid-tier suppliers show lower reject rates with similar SRI | Spend allocation is not fully optimized for quality. Shifting volume toward lower-risk suppliers can reduce operational exposure. |
| 4️⃣ | **PPV Differences Are Limited Across Suppliers** | - PPV% remains relatively consistent (~**5%**)<br>- No strong link between PPV and lower reject rate | Small price advantages do not justify higher quality risk. Focusing only on cost savings may increase long-term operational costs. |
| 5️⃣ | **At-Risk Suppliers Can Be Identified Clearly** | - High-spend suppliers with high reject rates create elevated exposure<br>- Low-reject suppliers maintain stable SRI | Suppliers can be segmented into **Strategic**, **Monitor**, and **At-Risk** groups, enabling smarter vendor prioritization and risk management. |

**🎯 Executive Takeaway**

The supplier base is operationally reliable, but quality variation creates uneven risk exposure.

The main opportunity is to:

- Reduce dependency on high-reject suppliers  
- Increase allocation to consistent, low-risk vendors  
- Use performance-based segmentation to guide sourcing decisions

#### Product 

<img width="1452" height="812" alt="image" src="https://github.com/user-attachments/assets/79bcbde5-7a3c-4464-94ec-5aaf4ab02070" />

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
