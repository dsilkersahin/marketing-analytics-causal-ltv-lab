
# Phase 1 Retention Summary

## Dataset limitation
This dataset is customer-level and does not contain signup dates or transaction-level timestamps.
Therefore, true calendar cohort retention cannot be estimated.

## Proxy retention definitions
- retained_30d = Last_Transaction_Days_Ago <= 30
- dormant_90d = Last_Transaction_Days_Ago > 90

## Main outputs
- Activity-based retention comparison
- Segment-level retention comparison
- LTV-recency risk matrix

## Next step
Use these proxies to create a churn target and model churn risk.
