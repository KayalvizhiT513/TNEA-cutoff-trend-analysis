# 📊 TNEA Cutoff Trend Analysis
A deep dive into Tamil Nadu Engineering Admissions (TNEA) cutoff data, uncovering surprising trends in 7.5% Government School Reservation versus General category counseling between 2021 and 2024.

🔍 Project Overview
This repository explores the evolution of closing ranks in TNEA counseling, with a particular focus on how the 7.5% reservation for Government School students compares to the general category over the years.

The analysis aims to answer one central question:

Is there a consistent point in the college ranking where the 7.5% reservation cutoffs surpass general category cutoffs? If so, is this point shifting over time?

Spoiler: Yes — and it’s moving up. 🎯

📁 Repository Structure
bash
Copy
Edit
TNEA-cutoff-trend-analysis/
│
├── 📓 preprocessing.ipynb         # Data cleaning, filtering, and shaping from raw Excel sources
├── 📓 tnea_eda_viz.ipynb          # Exploratory Data Analysis and final visualization plots
├── 📄 README.md                   # This file
├── 📂 data/                       # [Optional] Source Excel sheets (not pushed to GitHub)
📌 Dataset Description
The analysis uses:

📄 Cutoff data (2021–2024) for CSE branch across all TNEA-participating colleges

📄 Public perception rankings (PP Rank) for each college

📄 Separate cutoffs for:

🧍 General Category

🏫 7.5% Government School Reservation

🧪 Steps of Analysis
1. Data Preprocessing
Extracted sheets from Excel files:

Average OC cutoffs (2021–2024)

Reservation cutoffs (2022–2024) for CSE

Cleaned missing data and removed anomalies ("Not found" values, zero cutoffs)

Standardized column names and filtered for 'BRANCH CODE' == 'CS'

📓 See: preprocessing.ipynb

2. Exploratory Data Analysis (EDA)
Created scatter plots of OC Closing Rank vs Public Perception Rank

Compared general vs 7.5% reservation across years

Applied linear regression to each category per year

Identified intersection points: where reservation cutoffs overtake general cutoffs

Observed a clear upward shift in crossover points over the years

📓 See: tnea_eda_viz.ipynb

💡 Key Insights
Each year, there is a college PP rank where the reservation closing ranks start to become higher than general.

This cutoff intersection point is moving up the perception rank scale — meaning more highly ranked colleges are seeing reservation students closing earlier.

This suggests that reservation category students are opting or getting placed in better-ranked colleges year over year — a positive shift in access equity.

📈 Visual Highlight
The final visual in the notebook shows all three years (2022–2024) overlaid with regression lines and intersection points:

📉 Blue dashed lines: General trend

🟧 Orange dashed lines: 7.5% Reservation trend

🔴 Intersection markers: Crossover points

The rising trend of intersection tells a story of shifting dynamics in the TNEA landscape.

🤔 Why This Matters
Understanding these trends is critical for:

Policymakers monitoring the impact of reservation policies

Students and parents navigating college options

Researchers and educators tracking access to higher education

📌 Future Plans
Expand analysis to other branches (ECE, MECH, etc.)

Use clustering or polynomial fits to explore non-linear patterns

Build an interactive dashboard for year-wise counseling simulation

