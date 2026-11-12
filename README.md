# Databricks ML Professional Project

An end-to-end MLOps project on Databricks Free Edition, built to practice the skills covered by the Databricks Certified Machine Learning Professional exam.

## Goal

Predict NYC taxi fares from trip data, then build the surrounding production workflow: feature management, experiment tracking, model registry with aliases, batch and real-time deployment, orchestration with Jobs and Asset Bundles, and monitoring with retraining triggers.

## Dataset

- **Phase 0 sample:** `samples.nyctaxi.trips`, 21,932 trips from 1 Jan to 29 Feb 2016. Used for setup and validation.
- **Phase 1 onward:** NYC TLC yellow taxi trip records (monthly Parquet files), covering a longer window to support time-based splits and drift monitoring.

## Environment

- Databricks Free Edition, serverless compute only
- Unity Catalog, three-level namespace: `<catalog>.taxi.<table>`
- Delta tables throughout
- MLflow for tracking and the model registry

## Repository layout

```
├── README.md
└── notebooks/
    └── phase0_setup.py        # Phase 0 notebook
```

Notebooks and docs live in subfolders. Config files such as `databricks.yml` (from Phase 5) stay in the root.

## Roadmap

| Phase | Focus | Status |
|---|---|---|
| 0 | Setup and data access | In progress |
| 1 | Data and features (point-in-time-safe) | Not started |
| 2 | Training and experiment tracking | Not started |
| 3 | Model registry and governance | Not started |
| 4 | Deployment (batch and real-time) | Not started |
| 5 | Orchestration and CI/CD | Not started |
| 6 | Monitoring and retraining | Not started |
