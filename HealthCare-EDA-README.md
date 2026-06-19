# Healthcare EDA — Northampton Council Health Investigation

**An exploratory analysis of a 55,000-record healthcare dataset to identify the most common
medical conditions in a town, who they affect, and how the council might respond.**

> A business-framed EDA: structured around the questions a town council would actually ask,
> answered with visual analysis, demographic breakdowns, and interactive charts.

---

## Business problem
Northampton (hypothetical) has seen a rise in sickness and hospital admissions. The town council
commissioned diagnostic research to identify the underlying causes and shape mitigation strategy.
This project investigates the data behind that brief.

## Objectives
- What are the most common medical conditions in the town?
- Which demographics (age, gender, blood type) are most affected?
- How do conditions vary across hospitals and over time?
- What can the council do to mitigate them?

## Dataset
~55,500 patient records across 14 fields — demographics, medical condition, admission/discharge
details, billing, hospital, and test results. Source: Kaggle.

## What I did
- **Cleaning:** dropped identifying/irrelevant columns (name, doctor, room number), checked for
  nulls, standardised values, rounded billing amounts
- **EDA:** condition frequency, demographic breakdowns, hospital comparisons, and time trends
- **Interactive visuals:** built `ipywidgets` controls (toggle charts by gender, blood type, test
  result) and an `ipyleaflet` map view for richer exploration
- **Interpretation:** paired each chart with plain-English findings and domain reasoning
- **Recommendations:** translated the patterns into council-level actions

## Key findings
- Identified the most prevalent conditions and the demographics most associated with each
- Surfaced gender- and age-linked patterns in specific conditions
- Compared condition prevalence across hospitals to highlight where to focus resources

## Tools
Python (pandas, seaborn, matplotlib, ipywidgets, ipyleaflet)

> **Note:** the interactive widgets don't render in GitHub's static preview. Key charts are
> included as screenshots in `/Images`; clone and run locally for the full interactive version.

---

## Planned upgrade
- Add a predictive layer (e.g., classify likely condition from demographics) to move from
  descriptive to predictive analysis
