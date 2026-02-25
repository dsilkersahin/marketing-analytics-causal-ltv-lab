# Marketing Analytics Causal & LTV Lab

## Overview

This repository demonstrates applied marketing analytics and AdTech modeling techniques focused on:

- Incremental revenue estimation
- Uplift modeling
- Cohort & retention analysis
- Lifetime value (LTV) prediction
- Difference-in-Differences (DiD)
- Media Mix Modeling (MMM)
- KPI optimization frameworks

The objective is to simulate real-world AdTech and Growth Analytics decision-making scenarios using reproducible pipelines and business-oriented evaluation metrics.

---

## Business Motivation

Modern marketing analytics requires moving beyond correlation and optimizing for:

- Incremental revenue
- Sustainable retention
- Efficient CAC allocation
- Budget optimization
- Campaign incrementality

This lab focuses on **causal reasoning and revenue ownership**, rather than vanity metrics.

---

## Project Structure
```
marketing-analytics-causal-ltv-lab/
├── src/                              # Main source code
│   ├── evaluation/                    # Business & model evaluation logic
│   │   ├── uplift_metrics.py          # Qini, uplift curves, CATE evaluation
│   │   ├── retention_metrics.py       # Retention & survival metrics
│   │   ├── kpi_simulation.py          # KPI sensitivity & what-if analysis
│   │   └── revenue_simulator.py       # Incremental revenue simulation
│   │
│   ├── models/                        # Model implementations
│   │   ├── ltv/                       # Lifetime value models
│   │   │   ├── regression.py          # LTV regression models
│   │   │   ├── feature_pipeline.py    # Early behavior feature engineering
│   │   │   └── segmentation.py        # LTV-based user segmentation
│   │   │
│   │   ├── churn/                     # Retention & churn models
│   │   │   ├── classification.py      # Churn classification models
│   │   │   └── survival.py            # Survival analysis (Kaplan-Meier, Cox)
│   │   │
│   │   ├── uplift/                    # Uplift modeling
│   │   │   ├── t_learner.py           # T-learner implementation
│   │   │   ├── x_learner.py           # X-learner implementation
│   │   │   └── causal_forest.py       # Causal forest approach
│   │   │
│   │   ├── causal/                    # Causal inference methods
│   │   │   ├── difference_in_differences.py  # DiD implementation
│   │   │   ├── propensity_matching.py        # PSM
│   │   │   └── synthetic_control.py          # Synthetic control method
│   │   │
│   │   └── mmm/                       # Media Mix Modeling
│   │       ├── adstock.py             # Adstock transformation
│   │       ├── saturation.py          # Diminishing returns modeling
│   │       └── bayesian_mmm.py        # Bayesian MMM (PyMC)
│   │
│   ├── preprocessing/                 # Data preprocessing utilities
│   │   ├── cohort_builder.py          # Cohort construction logic
│   │   ├── feature_engineering.py     # Marketing feature pipelines
│   │   ├── spend_transformations.py   # Adstock & scaling transforms
│   │   └── splitting.py               # Time-aware data splits
│   │
│   └── utils/                         # Utility functions
│       ├── config.py                  # Configuration management
│       ├── plotting.py                # Executive-style visualizations
│       └── reproducibility.py         # Random seed & experiment control
│
├── notebooks/                         # Jupyter notebooks for analysis
│   ├── 01_cohort_retention.ipynb      # Cohort & retention analysis
│   ├── 02_ltv_prediction.ipynb        # LTV modeling & CAC simulation
│   ├── 03_uplift_modeling.ipynb       # Uplift modeling experiments
│   ├── 04_difference_in_differences.ipynb  # Campaign incrementality
│   ├── 05_kpi_optimization.ipynb      # KPI tree & sensitivity analysis
│   └── 06_media_mix_model.ipynb       # Budget allocation modeling
│
├── data/                              # Data directory
│   ├── raw/                           # Original datasets
│   ├── processed/                     # Cleaned datasets
│   └── synthetic/                     # Synthetic marketing datasets
│
├── experiments/                       # Experiment results & tracking logs
├── reports/                           # Business summaries & insights
│   ├── executive_summary.md
│   └── revenue_impact_report.md
│
├── tests/                             # Unit tests for core modules
├── requirements.txt                   # Python dependencies
├── pyproject.toml                     # Project configuration
└── README.md
```

## Modules & Capabilities

### 1. Cohort & Retention Analysis
- Monthly cohort retention matrices
- Channel-based retention comparison
- Kaplan-Meier survival curves
- Revenue decay modeling

### 2. LTV Prediction
- Early behavior feature engineering (first 7–14 days)
- 180-day LTV regression modeling
- Customer segmentation by predicted LTV
- CAC vs LTV profitability simulation

### 3. Uplift Modeling
- T-Learner and X-Learner implementations
- Conditional Average Treatment Effect (CATE)
- Qini curve and uplift curve evaluation
- Incremental revenue targeting simulation

### 4. Difference-in-Differences (DiD)
- Campaign incrementality analysis
- Parallel trend validation
- Confidence interval estimation
- ROI calculation

### 5. Media Mix Modeling (MMM)
- Adstock transformation
- Diminishing returns modeling
- Channel elasticity estimation
- Budget reallocation simulation

---

## Business Simulation Framework

This lab includes revenue simulation utilities to evaluate:

- Blanket targeting vs uplift-based targeting
- Retention campaign profitability
- Channel-based CAC efficiency
- Budget reallocation impact on total revenue

All evaluations are framed in terms of **incremental revenue impact**.

---

## Example Business Questions Addressed

- Which acquisition channel produces the highest long-term LTV?
- What is the incremental ROI of paid search?
- Should discounts be given to all users or only high-uplift segments?
- How does improving retention by 3% impact total revenue?
- What is the optimal marketing budget distribution across channels?

---

## Installation

Create a virtual environment:

```bash
python -m venv venv
source venv/bin/activate        # Mac/Linux
venv\Scripts\activate           # Windows

pip install -r requirements.txt