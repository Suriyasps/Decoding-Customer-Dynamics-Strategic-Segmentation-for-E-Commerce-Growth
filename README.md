# Decoding Customer Dynamics: Strategic Segmentation for E-Commerce Growth

# Marketing Analytics  
**Proejct By**: Suriya Subbiah Perumal  

---

## 📌 Overview

This project presents an in-depth segmentation study for a multinational e-commerce retailer specializing in unique gifts. With a diverse customer base including wholesalers, the goal was to identify meaningful customer segments using advanced analytics.

The methodology integrates:
- **Hierarchical & K-means Clustering**
- **Discriminant Analysis**
- **RFM (Recency-Frequency-Monetary) Analysis**

---

## 🧭 Methodology (CRISP-DM Framework)

### 1. Business Understanding
Target segments for tailored marketing strategies that maximize ROI.

### 2. Data Understanding
- Data from 10,000 transactions (01-Dec-2020 to 24-Nov-2021)
- Included both **demographic** and **transactional** fields

### 3. Data Preparation
- Data cleaning (e.g., replacing NAs, dummy encoding)
- Variable scaling
- Dummy coding for categorical clustering compatibility

### 4. Modeling Techniques
- **Hierarchical Clustering**: Four linkage methods explored (Complete, Single, Average, Centroid)
- **K-means Clustering**: Optimal k=3; results improved significantly with `nstart=50`
- **Discriminant Analysis**: LDA models with ANOVA validation
- **RFM Analysis**: Segmentation based on purchasing behavior

---

## 📊 Key Insights

### 📈 Hierarchical Clustering
- **Elbow plot** consistently suggested 3 clusters.
- Complete linkage proved most effective for initial segmentation.

### 📌 K-means Clustering
- Cluster separation improved with increased `nstart` values (tested at 1, 10, 25, 50).
- Final model with `nstart=50` offered best within-cluster vs between-cluster variance.

### 🧠 Discriminant Analysis
- Used demographic traits like **Age**, **Income**, **Education**.
- LD2 showed statistical significance (p < 0.1) — a key differentiator for segment 3.
- Suggested **high-income, experienced** customers as prime targets.

---

## 📦 RFM Analysis

### RFM Dimensions:
- **Recency**: Days since last purchase
- **Frequency**: Count of unique invoices
- **Monetary**: Total spend

### Key Findings:
- Customers in segment **R1-F3-M3** had the **highest monetary value** despite lower frequency.
- This segment represents **low engagement, high value** — ideal for **targeted reactivation campaigns**.

---

## 🎯 Targeted Marketing Strategy

- Prioritize **R1-F3-M3** for campaigns: infrequent but lucrative buyers.
- Use **personalized incentives**, loyalty programs, and email marketing to boost frequency.
- Aligns with Sharp & Sharp (1997) on loyalty-driven profitability.

---

## 🛠 Tools & Techniques Used

- **Languages**: R (clustering, discriminant analysis), Tableau (visualizations)
- **Libraries**: `dplyr`, `MASS`, `fastDummies`, `lubridate`
- **Segmentation Models**: `hclust`, `kmeans`, `lda`
- **Customer Value Modeling**: RFM scores (Independent & Sequential sort)

---

## 🧠 Academic Frameworks Referenced

- Hair et al. (2014), Tabachnick & Fidell (2013): Statistical modeling
- Ketchen & Shook (1996), Tibshirani et al. (2001): Clustering best practices
- Rousseeuw (1987): Silhouette analysis
- Blattberg & Deighton (1996): Customer equity in marketing

---

## ✅ Conclusion

This project successfully demonstrates how combining **statistical clustering techniques** with **behavioral segmentation models** can uncover deep customer insights. Segment 3 (R1-F3-M3) emerges as a strategic opportunity for high-ROI marketing interventions.

The approach balances **modeling rigor** with **marketing relevance**, empowering e-commerce companies to implement data-driven strategies.

---

## 📌 Future Work

- Add psychographic variables to enhance segmentation
- Incorporate LLM-powered NLP to cluster based on customer reviews or service chats
- Automate the segmentation pipeline for dynamic personalization

