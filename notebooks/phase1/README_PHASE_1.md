# Phase 1 Notebooks — Customer Analytics, Churn and LTV Baseline

Use these notebooks with:

```text
data/raw/digital_wallet_ltv_dataset.csv
```

Recommended order:

1. `01_data_quality_and_eda.ipynb`
2. `02_cohort_retention_analysis.ipynb`
3. `03_churn_analysis.ipynb`
4. `04_ltv_prediction.ipynb`
5. `05_ltv_segmentation_and_business_simulation.ipynb`

The notebooks are designed to be run step by step. Each notebook includes discussion prompts so we can review the outputs together and connect the code to interview-level explanations.

Important limitation: this dataset is customer-level and does not include transaction timestamps, signup dates, campaign exposure, treatment assignment, or marketing spend time series. So Phase 1 is a baseline customer analytics layer, not causal inference yet.
