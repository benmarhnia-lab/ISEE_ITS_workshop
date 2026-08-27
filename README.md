# Interrupted Time Series Analysis in Environmental Epidemiology

Materials for the ISEE 2026 pre-conference workshop: **Interrupted Time Series Analysis in Environmental Epidemiology: An Overview of Traditional and Novel Modeling Approaches**

**Instructors:** Tarik Benmarhnia and Yiqun Ma

The repository contains the workshop slides, datasets, rendered HTML documents, and R Markdown source files.

## Learning objectives

By the end of the workshop, participants should be able to:

1. Explain when an ITS design may be appropriate.
2. Define the target counterfactual for a clearly timed environmental event.
3. Fit and interpret a classical segmented-regression ITS model.
4. Explain the logic of a two-stage machine learning-integrated ITS design.
5. Describe how an ITS framework can be extended to multiple events and meta-regression.

## Workshop materials

| Part | Topic | Format during workshop |
| --- | --- | --- |
| 1 | Introduction to the San Francisco case study and dataset | Live coding |
| 2 | Classical ITS with segmented regression | Live coding |
| 3 | Two-stage machine learning-integrated ITS | Pre-rendered walkthrough |
| 4 | Extension to multiple events and meta-regression | Live coding |

The corresponding rendered HTML documents are:

- `01_case_study_and_data.html`
- `02_classical_ITS_segmented_regression.html`
- `03_ML_ITS_workflow.html`
- `04_multiple_event_meta_regression.html`


## Software setup

We recommend a recent version of R and RStudio Desktop.

### Required packages for Parts 1, 2, and 4

The following packages are needed for the live-coding portions: "tidyverse", "patchwork", "scales", "tsModel", "mvmeta", "knitr", "rmarkdown"


### Optional packages for Part 3

Part 3 uses a Prophet–XGBoost model and is provided mainly as a pre-rendered walkthrough.

You do **not** need these packages for the live-coding portions. To run the Part 3 workflow independently, install: "timetk", "lubridate", "tidymodels", "modeltime", "Metrics", "prophet", "xgboost", "rstan", "QuickJSR"


## Data files

The analyses use two R data files:

- `data_case_study_11to18.RDS`: daily San Francisco case-study data used in Parts 1–3.
- `multiple_event_data.RDS`: simulated event-level data used in Part 4.

## Reference

The workshop is based on concepts described in:

> Ma, Y., & Benmarhnia, T. (2025). Interrupted time series analysis in environmental epidemiology: A review of traditional and novel modeling approaches. *Current Environmental Health Reports, 12*(1), 50. <https://doi.org/10.1007/s40572-025-00517-3>
> Dey, A. K., Ma, Y., Carrasco-Escobar, G., Han, C., Rerolle, F., & Benmarhnia, T. (2025). Two-stage interrupted time series analysis with machine learning: Evaluating the health effects of the 2018 wildfire smoke event in San Francisco County as a case study. *American Journal of Epidemiology, 194*(10), 2936–2944. <https://doi.org/10.1093/aje/kwaf147>

## Questions and feedback

For questions about the workshop materials, please contact:

- [Yiqun Ma, yiqunma@ucsd.edu]
