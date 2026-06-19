# Marketing Analytics Causal & LTV Lab

## Overview

This repository demonstrates applied marketing analytics, experimentation, causal inference, and growth modeling techniques focused on measuring true business impact rather than observational correlation.

Core topics include:

* Cohort & retention analysis
* Customer Lifetime Value (LTV) prediction
* Churn modeling & survival analysis
* A/B testing & experimentation
* Uplift modeling
* Causal inference
* Difference-in-Differences (DiD)
* Synthetic Control
* Media Mix Modeling (MMM)
* Budget allocation & KPI optimization

The repository combines real-world datasets and synthetic simulations to reproduce common marketing analytics challenges such as selection bias, treatment leakage, seasonality, attribution errors, multicollinearity, and experiment design pitfalls.

The objective is to simulate real-world Growth Analytics, Marketing Science, and AdTech decision-making environments using reproducible pipelines, business-oriented evaluation metrics, and causal reasoning frameworks.

---

## Business Motivation

Modern growth and marketing organizations must answer questions that go beyond prediction:

* Did the campaign actually cause incremental revenue?
* Which customers should receive incentives?
* How should marketing budgets be allocated?
* Which acquisition channels generate sustainable long-term value?
* How can experimentation be trusted at scale?

This lab focuses on measuring causal impact and business value through a combination of experimentation, causal inference, predictive modeling, and optimization frameworks.

All analyses are evaluated through business KPIs such as:

* Incremental revenue
* Incremental conversions
* Customer Lifetime Value (LTV)
* Retention
* CAC efficiency
* Marketing ROI

---

## Project Structure

```text
marketing-analytics-causal-ltv-lab/

├── src/
│
│   ├── evaluation/
│   │   ├── uplift_metrics.py
│   │   ├── retention_metrics.py
│   │   ├── kpi_simulation.py
│   │   └── revenue_simulator.py
│   │
│   ├── models/
│   │
│   │   ├── ltv/
│   │   │   ├── regression.py
│   │   │   ├── feature_pipeline.py
│   │   │   └── segmentation.py
│   │   │
│   │   ├── churn/
│   │   │   ├── classification.py
│   │   │   └── survival.py
│   │   │
│   │   ├── experimentation/
│   │   │   ├── ab_test.py
│   │   │   ├── power_analysis.py
│   │   │   ├── cuped.py
│   │   │   ├── sequential_testing.py
│   │   │   └── srm_detection.py
│   │   │
│   │   ├── uplift/
│   │   │   ├── t_learner.py
│   │   │   ├── x_learner.py
│   │   │   └── causal_forest.py
│   │   │
│   │   ├── causal/
│   │   │   ├── difference_in_differences.py
│   │   │   ├── propensity_matching.py
│   │   │   └── synthetic_control.py
│   │   │
│   │   └── mmm/
│   │       ├── adstock.py
│   │       ├── saturation.py
│   │       └── bayesian_mmm.py
│   │
│   ├── preprocessing/
│   │   ├── cohort_builder.py
│   │   ├── feature_engineering.py
│   │   ├── spend_transformations.py
│   │   └── splitting.py
│   │
│   └── utils/
│       ├── config.py
│       ├── plotting.py
│       └── reproducibility.py
│
├── notebooks/
│   ├── 01_cohort_retention.ipynb
│   ├── 02_ltv_prediction.ipynb
│   ├── 03_ab_testing.ipynb
│   ├── 04_uplift_modeling.ipynb
│   ├── 05_difference_in_differences.ipynb
│   ├── 06_media_mix_model.ipynb
│   └── 07_budget_optimization.ipynb
│
├── data/
│   ├── raw/
│   │   ├── digital_wallet_ltv_dataset.csv
│   │   ├── marketing_ab_testing.csv
│   │   └── criteo_uplift.csv
│   │
│   ├── processed/
│   │
│   └── synthetic/
│       ├── synthetic_mmm_weekly.csv
│       ├── synthetic_did_regions.csv
│       ├── synthetic_ab_edge_cases.csv
│       └── synthetic_marketing_environment.csv
│
├── experiments/
│
├── reports/
│   ├── executive_summary.md
│   ├── revenue_impact_report.md
│   └── business_recommendations.md
│
├── tests/
│
├── requirements.txt
├── pyproject.toml
└── README.md
```

---

## Data Sources

The project combines real-world public datasets with synthetic simulations.

### Real Datasets

#### Digital Wallet LTV Dataset

Used for:

* Cohort analysis
* Retention analysis
* Customer segmentation
* Churn prediction
* LTV modeling

Key fields include:

* Transaction behavior
* Engagement metrics
* Loyalty activity
* Customer satisfaction
* Historical LTV

#### Criteo Uplift Dataset

Used for:

* Treatment effect estimation
* Incrementality analysis
* Uplift modeling
* CATE estimation

#### Marketing A/B Testing Dataset

Used for:

* Experiment analysis
* Conversion lift estimation
* Statistical testing
* Experiment validation

### Synthetic Datasets

Several synthetic datasets are generated to reproduce scenarios rarely available in public data.

Examples include:

* Weekly marketing channel spend
* Campaign interventions
* Geographic experiments
* Treatment assignment
* Incrementality scenarios
* Budget allocation simulations

---

## Modules & Capabilities

### 1. Cohort & Retention Analysis

* Monthly cohort retention matrices
* Retention curves
* Revenue retention analysis
* Kaplan-Meier survival estimation
* Retention decomposition by acquisition channel

### 2. LTV Prediction

* Early behavior feature engineering
* LTV regression models
* Customer segmentation
* CAC-to-LTV profitability analysis
* Revenue forecasting by customer segment

### 3. Churn Modeling

* Churn classification
* Survival analysis
* Hazard estimation
* Retention intervention targeting
* Churn risk segmentation

### 4. A/B Testing & Experimentation

* Frequentist hypothesis testing
* Power analysis
* Sample size estimation
* CUPED variance reduction
* Sequential testing
* Sample Ratio Mismatch (SRM) detection

### 5. Uplift Modeling

* T-Learner
* X-Learner
* Causal Forest
* Conditional Average Treatment Effect (CATE)
* Uplift targeting simulations
* Incremental revenue optimization

### 6. Causal Inference

* Difference-in-Differences
* Propensity Score Matching
* Synthetic Control
* Incrementality measurement
* Policy and intervention evaluation

### 7. Media Mix Modeling (MMM)

* Adstock transformation
* Saturation modeling
* Bayesian MMM
* Channel elasticity estimation
* Marketing attribution analysis
* Budget allocation optimization

### 8. KPI Optimization

* Revenue sensitivity analysis
* KPI trees
* Scenario simulation
* Marketing budget optimization
* Executive-level impact estimation

---

## Edge Cases & Pitfalls Covered

The repository intentionally reproduces common analytical mistakes and business challenges.

### Experimentation

* Underpowered experiments
* Sample Ratio Mismatch (SRM)
* Peeking bias
* Multiple hypothesis testing
* Novelty effects
* Instrumentation failures

### Causal Inference

* Selection bias
* Confounding variables
* Parallel trend violations
* Treatment contamination
* Hidden confounders

### Media Mix Modeling

* Multicollinearity
* Adstock effects
* Saturation effects
* Delayed channel impact
* Seasonality leakage
* Budget shocks

### LTV & Churn

* Feature leakage
* Survivorship bias
* Incomplete cohorts
* Data drift
* Target leakage

---

## Business Simulation Framework

The repository contains simulation utilities that evaluate business decisions rather than only model performance.

Examples include:

* Blanket targeting vs uplift targeting
* Retention campaign profitability
* CAC efficiency by acquisition channel
* Revenue impact of churn reduction
* Incremental revenue estimation
* Marketing budget reallocation

All evaluations are framed through business outcomes rather than solely predictive metrics.

---

## Example Business Questions Addressed

### Experimentation

* Is the observed lift statistically significant?
* Is the lift practically meaningful?
* Was the experiment correctly randomized?
* Can the results be trusted?

### Causal Inference

* What is the true incremental impact of a campaign?
* Which users convert because of the intervention?
* What would have happened without the treatment?

### Growth Analytics

* Which acquisition channels generate the highest long-term value?
* Which customers should receive retention incentives?
* Which users should receive discounts?

### Media Mix Modeling

* What is the ROI of each marketing channel?
* Which channels drive the strongest marginal returns?
* How should marketing budgets be redistributed?

### Executive Decision Making

* What is the revenue impact of increasing retention by 3%?
* What is the expected value of a new retention campaign?
* How should a fixed marketing budget be allocated?

---

## Learning Objectives

This repository is designed to provide hands-on experience with:

* Marketing Analytics
* Growth Analytics
* Product Analytics
* Experimentation Platforms
* Causal Inference
* Bayesian Modeling
* Customer Lifetime Value Modeling
* Marketing Science
* Decision Intelligence

The focus is not only on building models, but also on understanding when models fail, how bias is introduced, and how to make reliable business decisions under uncertainty.

---

## Installation

```bash
python -m venv venv

source venv/bin/activate      # Mac/Linux
venv\Scripts\activate         # Windows

pip install -r requirements.txt
```

---

## Future Extensions

Planned additions:

* Multi-touch attribution modeling
* Double Machine Learning (DML)
* Bayesian A/B testing
* Thompson Sampling
* Contextual Bandits
* Reinforcement Learning for budget allocation
* Causal Graphs (DAGs)
* Marketing Mix Optimization
* GeoLift experiments
* Incrementality testing framework
* Customer Journey Analytics
* Agent-based marketing simulations

```
```
