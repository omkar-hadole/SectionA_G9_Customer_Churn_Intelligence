<div align="center">

# 🏦 Customer Churn Intelligence in Banking

### DVA Capstone 2 — Data Visualization & Analytics | Newton School of Technology (RU)

[![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Tableau](https://img.shields.io/badge/Tableau-Public-E97627?style=for-the-badge&logo=tableau&logoColor=white)](https://public.tableau.com/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Sector](https://img.shields.io/badge/Sector-Banking%20%26%20Financial%20Services-22c55e?style=for-the-badge)]()

---

**Section A · Group 9 · Submission Date: 29 April 2026**

</div>

---

## 👥 Team Members

| Name | Student ID | Contribution |
|------|-----------|-------------|
| **Omkar Hadole** | 24010101252 | ETL & Cleaning, EDA & Analysis |
| **Mayank Yadav** | 24010100008 | Statistical Analysis, Report Writing |
| **Sarvjeet Yadav** | 24010102271 | Dataset & Sourcing, EDA & Analysis |
| **Lakshya Bapna** | 24010101424 | Tableau Dashboard, PPT & Viva |
| **Debasish Karan** | 24010101175 | Tableau Dashboard, Report Writing |
| **Aarya Srivastava** | 24010101141 | Dataset & Sourcing, PPT & Viva |

**Faculty Mentor:** Satyaki Das  
**Team ID:** Group 9  

---

## 📌 Problem Statement

> *"What key customer behavioural and financial factors influence churn in a banking system, and how can high-risk customers be identified early enough for effective retention intervention?"*

Customer churn is a major concern in the banking sector as it directly impacts revenue and long-term customer value. Banks lose substantial income when customers close accounts and switch to competitors — and the cost of acquiring a replacement customer far exceeds that of retaining an existing one.

This project addresses the challenge of **identifying the key behavioural and financial factors that drive churn**, enabling early intervention before customers leave.

---

## 💡 Solution

The project delivered an end-to-end descriptive and diagnostic analytics pipeline:

1. **Data Ingestion & ETL** — A customer-level banking dataset of ~28,000 records was sourced, cleaned, and preprocessed using Python.
2. **KPI Engineering** — Derived KPIs including Churn Rate, Active Rate, Average Balance, and Balance Change were computed from raw fields.
3. **Exploratory Data Analysis (EDA)** — Patterns across activity status, tenure, balance trends, and risk segments were uncovered through structured visual and statistical analysis.
4. **Statistical Validation** — Hypothesis testing (chi-square), correlation analysis (point-biserial), distribution analysis, and anomaly detection were applied to validate findings.
5. **Interactive Dashboards** — Three Tableau dashboards translate analytical findings into accessible, decision-ready tools for non-technical stakeholders.

### 🔑 Key Insights

- 🔴 **Inactive customers** churn at significantly higher rates than their active counterparts.
- 🟠 **New customers (0–2 year tenure)** represent the highest-risk churn cohort.
- 🟡 Customers with **declining account balances** show a strong propensity to churn.
- 🔵 **High-risk customer segments** exhibit disproportionately elevated churn rates across all metrics.
- Account balance and tenure show the **strongest negative correlations** with churn — higher balance and longer tenure significantly reduce churn likelihood.

### ✅ Key Recommendations

| # | Recommendation | Estimated Churn Reduction |
|---|---------------|--------------------------|
| 1 | Deploy early engagement campaigns for new customers (0–2 yr) | 10–20% of early-stage churn |
| 2 | Implement automated balance-decline alerts for proactive outreach | 5–15% of balance-driven churn |
| 3 | Launch reactivation programs for inactive customers | 8–15% reactivation rate |
| 4 | Develop personalized retention plans for high-risk segments | 15–25% of high-risk churn |
| 5 | Create occupation-specific financial products to reduce financial stress | Opens new revenue streams |

---

## 🛠️ Tech Stack & Tools Used

| Category | Tools / Libraries |
|----------|------------------|
| **Language** | Python 3.10+ |
| **Data Processing** | Pandas, NumPy |
| **Statistical Analysis** | SciPy (chi-square, point-biserial correlation) |
| **Visualization (Python)** | Matplotlib, Seaborn |
| **Business Intelligence** | Tableau Public |
| **Notebooks** | Jupyter Notebook |
| **ETL Pipeline** | Custom Python script (`scripts/etl_pipeline.py`) |
| **Version Control** | Git & GitHub |
| **Outlier Handling** | IQR-based winsorization |
| **Missing Value Strategy** | Median (numeric) / Mode (categorical) imputation |

---

## 📊 Tableau Dashboards

Three interactive dashboards were designed, each serving a distinct business question:

| Dashboard | Business Question | Key Visualizations |
|-----------|------------------|--------------------|
| **1. Behavior Analysis** | *Why are customers churning?* | Activity vs. Churn, Tenure vs. Churn, Balance Decline Analysis |
| **2. Customer Segmentation** | *Who is at risk?* | Risk Segmentation Breakdown, Age Group Heatmap, Occupation Breakdown |
| **3. Customer Value & Balance** | *What is the financial impact?* | Balance Distribution, Balance Change Analysis, Avg Balance by Segment |

> 🔗 Dashboard links are documented in [`tableau/dashboard_links.md`](./tableau/dashboard_links.md)

---

## 📁 Project Structure

```
SectionA_G9_Customer_Churn_Intelligence/
│
├── 📂 data/
│   ├── raw/                        # Original unprocessed dataset
│   └── processed/                  # Cleaned & feature-engineered data
│
├── 📂 notebooks/
│   ├── 01_extraction.ipynb         # Data sourcing & initial load
│   ├── 02_cleaning.ipynb           # Data cleaning & standardisation
│   ├── 03_eda.ipynb                # Exploratory Data Analysis
│   ├── 04_statistical_analysis.ipynb  # Hypothesis testing & correlations
│   └── 05_final_load_prep.ipynb    # Final export for Tableau
│
├── 📂 scripts/
│   └── etl_pipeline.py             # End-to-end ETL pipeline script
│
├── 📂 tableau/
│   └── dashboard_links.md          # Tableau Public dashboard URLs
│
├── 📂 docs/
│   └── data_dictionary.md          # Field definitions & metadata
│
├── 📂 reports/
│   ├── DVA_Capstone2_Report_Condensed.pdf   # Final project report
│   ├── presentation.pdf            # Project presentation slides
│   ├── project_report.pdf          # Full detailed report
│   └── kpi_summary.csv             # KPI summary output
│
├── 📂 DVA-focused-Portfolio/       # Portfolio artifacts
├── 📂 DVA-focused-Resume/          # Resume artifacts
│
└── README.md
```

---

## 📈 Dataset Overview

| Attribute | Detail |
|-----------|--------|
| **Records** | ~28,000 customer-level rows |
| **Sector** | Banking & Financial Services |
| **Target Variable** | `Churn Label` (Binary: 1 = Churned, 0 = Retained) |

### Key Features

| Field | Type | Description |
|-------|------|-------------|
| `Age` | Numeric | Customer age in years |
| `Gender` | Categorical | Customer's gender |
| `Occupation` | Categorical | Reported occupation category |
| `Tenure (Years)` | Numeric | Years the customer has held an account |
| `Account Balance` | Numeric | Current or average account balance |
| `Activity Status` | Categorical | Active / Inactive based on recent transactions |
| `Risk Segment` | Categorical | Low / Medium / High risk classification |
| `Churn Label` | Binary | 1 = Churned, 0 = Retained |

---

## 🔬 Analytics Pipeline

```
Raw Data
   │
   ▼
01_extraction.ipynb       ← Source & load dataset
   │
   ▼
02_cleaning.ipynb         ← Missing values, outliers, standardisation
   │
   ▼
03_eda.ipynb              ← Visual patterns, distributions, segment analysis
   │
   ▼
04_statistical_analysis.ipynb   ← Chi-square, correlation, anomaly detection
   │
   ▼
05_final_load_prep.ipynb  ← Export clean data for Tableau
   │
   ▼
Tableau Dashboards        ← Interactive decision-support tools
```

### Cleaning Steps Applied
- Churn labels standardised to binary integer format (1 = Churned, 0 = Retained)
- Activity Status values normalised to consistent categorical encoding (Active / Inactive)
- Categorical columns stripped of whitespace and converted to title case
- Missing values imputed using **median** (numeric) or **mode** (categorical) strategies
- Rows with missing churn labels were excluded from analysis
- Numeric fields (Balance, Age, Tenure) assessed via **IQR-based outlier detection** and capped at 1st/99th percentiles (winsorization)

---

## 📐 Project Scope

| In Scope | Out of Scope |
|----------|-------------|
| Descriptive & diagnostic analytics | Real-time data pipelines |
| KPI computation | Live CRM integration |
| Exploratory Data Analysis (EDA) | ML-based churn prediction models *(future scope)* |
| Tableau dashboard development | Time-series micro-level tracking |

---

## 🎯 Success Criteria

- ✅ Clear, evidence-based identification of the top churn drivers
- ✅ Actionable insights that map directly to retention strategies
- ✅ Three fully functional, publicly accessible Tableau dashboards with interactive filters

---

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn scipy jupyter
```

### Running the Notebooks
```bash
# Clone the repository
git clone <repository-url>
cd SectionA_G9_Customer_Churn_Intelligence

# Launch Jupyter
jupyter notebook

# Run notebooks in order:
# 01_extraction → 02_cleaning → 03_eda → 04_statistical_analysis → 05_final_load_prep
```

### Running the ETL Pipeline
```bash
python scripts/etl_pipeline.py
```

---

## 📋 Contribution Matrix

| Team Member | Dataset & Sourcing | ETL & Cleaning | EDA & Analysis | Statistical Analysis | Tableau Dashboard | Report Writing | PPT & Viva |
|-------------|:-----------------:|:--------------:|:--------------:|:--------------------:|:-----------------:|:--------------:|:---------:|
| Omkar Hadole | | ✓ | ✓ | | | | |
| Mayank Yadav | | | | ✓ | | ✓ | |
| Sarvjeet Yadav | ✓ | | ✓ | | | | |
| Lakshya Bapna | | | | | ✓ | | ✓ |
| Debasish Karan | | | | | ✓ | ✓ | |
| Aarya Srivastava | ✓ | | | | | | ✓ |

---

## 📜 License

This project was developed as part of the **DVA Capstone 2** coursework at **Newton School of Technology (RU)**. All rights reserved by the team and the institution.

---

<div align="center">

Made with ❤️ by **Group 9 — Section A**  
Newton School of Technology · Data Visualization & Analytics · SEM IV

</div>
