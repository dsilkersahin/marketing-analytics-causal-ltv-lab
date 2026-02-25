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
marketing-analytics-causal-ltv-lab/
- environment.yml
- requirements.txt
- README.md

- data/
	- synthetic_data_generator.py
	- raw/
	- processed/

- experiments/
	- config.yaml
	- experiment_tracking.md

- notebooks/

- reports/
	- business_case_notes.md
	- executive_summary.md

- src/
	- data/
		- loader.py
		- preprocessing.py
		- feature_engineering.py
	- evaluation/
		- kpi_simulation.py
		- retention_metrics.py
		- revenue_simulator.py
		- uplift_metrics.py
	- modeling/
		- churn_model.py
		- did_model.py
		- ltv_model.py
		- mmm_model.py
		- uplift_model.py
	- visualization/
		- cohort_plots.py
		- kpi_tree.py
		- mmm_plots.py
		- uplift_curves.py

---

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