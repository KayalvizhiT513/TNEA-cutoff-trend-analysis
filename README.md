# 📊 TNEA Cutoff Trend Analysis

A data-driven exploration of Tamil Nadu Engineering Admissions (TNEA) cutoff trends from **2022 to 2024**, focusing on how **public perception rank** correlates with the **closing ranks** under **general counseling** and **7.5% government school reservation**.

> 🔍 **Main Insight:**  
At every college, there is a tipping point where the **7.5% reservation cutoff becomes higher than the general OC cutoff** — and interestingly, this point is **climbing up** the public perception ranks **every year**.

---

## 📁 Repository Structure

- **`General_vs_7_5_Reservation_(Data_Preprocessing).ipynb`**  
   Prepares and filters the data from multiple Excel sources. Includes:
   - Filtering by branch (CSE)
   - Cleaning "Not found" or missing perception ranks
   - Structuring year-wise datasets
   - Removing zero cutoffs or outliers

- **`General_vs_7_5_Reservation_(EDA_and_Viz).ipynb`**  
   A comprehensive visual analysis notebook. Features:
   - Scatter plots of closing ranks vs public perception
   - Year-wise trends for both General and 7.5% reservation categories
   - **Linear regression fits** and **intersection points**
   - Multi-year overlay visualizations with trendlines and annotations

---

## 🧪 Steps in the Analysis

### 1. Data Collection & Preprocessing
- Used publicly available `.xlsx` files of TNEA closing ranks.
- Selected only **Computer Science (CS)** branches to narrow the scope.
- Cleaned inconsistent perception rank entries and filtered out invalid records.

### 2. Year-wise Analysis
- Compared **OC (General)** and **7.5% reservation** closing cutoff for 2022, 2023, and 2024.
- Used **Public Perception Rank (PP Rank)** as the x-axis — a proxy for college reputation.

### 3. Visualizations & Trends
- Generated scatter plots and overlaid **linear regression lines** to model the trend for each category.
- Calculated **intersection points** of the two trend lines for each year.
- Found that:
   - In early PP ranks (top colleges), general OC cutoffs are typically higher (i.e., more competitive).
   - After a certain college rank, **7.5% reservation cutoffs surpass general cutoffs**.
   - This **intersection point is moving up** in PP rank each year, showing a trend of students in the 7.5% reservation category are outperforming more peers and competing closer to or beyond general category levels.

### 4. Key Insight
> 📈 The **cutoff reversal point** (where 7.5% reservation cutoffs exceed general OC cutoffs) is **shifting upward** in public perception ranks — meaning this phenomenon is happening at **more competitive colleges each year.**
> 🎯 This reflects **a rise in competitiveness** among government school students, who are securing admission to higher-ranked institutions, **even beyond the general counseling cutoffs** in some cases.
---

## ✨ Future Work

- Extend to other branches (ECE, MECH, etc.)
- Compare with **community-based reservations** and **first-generation graduate schemes**.
- Integrate admission trends with **HSC performance data**.

---
