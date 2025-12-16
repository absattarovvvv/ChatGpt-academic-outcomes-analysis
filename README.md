# Analyzing the ChatGPT effect: academic outcomes before and after LLM introduction

## Overview

This project examines how academic grade outcomes evolved before and after the introduction of large language models (LLMs), with a particular focus on ChatGPT. Using institutional grading data from SDU University across multiple academic years and departments, the analysis explores changes in grade distributions over time and investigates whether these changes differ across academic disciplines.

The study is exploratory and descriptive in nature, relying on structured exploratory data analysis (EDA) to identify patterns, trends, and heterogeneity in academic outcomes rather than to establish causal effects.

---

## Research Questions

- How did academic grade distributions change before and after the introduction of large language models?
- Were observed changes uniform across departments, or did certain disciplines exhibit different outcome dynamics?
- Did changes primarily affect high-performing, mid-range, or failing outcomes?

---

## Data

The analysis uses institutional grading data from **SDU University**, covering multiple semesters across the **2021–2023 academic years**.

**Timeframe definition:**
- **Pre-LLM period:** 2021–2022 academic year  
- **Transition period:** Fall 2022  
- **Post-LLM period:** Spring and Fall 2023  

**Scope and structure:**
- Unit of analysis: aggregated course–semester outcomes  
- Key variables: grade counts (A, B, C, D, FFX), department, academic year, semester  
- Departments included:
  - **MDE** — Language education department serving students from all faculties
  - **PED** — Education & Humanities
  - **ENG** — Engineering & Natural Sciences
  - **LAW** — Law & Social Sciences
  - **BS** — Business School

---

## Data Privacy & Ethics

The original datasets were accessed and analyzed within an academic research context under faculty supervision.  
All datasets shared publicly in this repository have been **fully anonymized**, with identifiable attributes replaced by consistent numeric encodings. No personally identifiable information is included.

The analysis focuses exclusively on **aggregate patterns**, and no individual-level inferences are made.

---

## Methodology

The analysis follows a structured exploratory data analysis workflow:

- Data cleaning, transformation, and aggregation are performed within the notebook
- Grade counts are normalized into proportions to enable comparison across semesters with different cohort sizes
- Grades are grouped into outcome bands:
  - **High performance:** A–B  
  - **Mid-range performance:** C–D  
  - **Failure:** FFX
- Trends are analyzed across time, departments, and pre/post LLM periods
- Visualizations include proportional heatmaps, trend lines, department-level comparisons, and baseline deviation (Δ-change) analysis

No predictive modeling or machine learning methods are used, as the project is intentionally focused on descriptive and comparative analysis.

---

## Key Findings

- Across the full sample, the share of high-performing outcomes (A–B) increased modestly over time by approximately **2–3 percentage points**, while failure outcomes (FFX) declined by a similar magnitude.
- Mid-range outcomes (C–D) remained largely stable throughout the observation period, indicating that changes were concentrated at the upper and lower ends of the grade distribution.
- Comparison of pre-LLM (2021–2022) and post-LLM (2023) periods shows a small shift toward higher outcomes and fewer failures, with no abrupt structural break.
- Department-level analysis reveals substantial heterogeneity:
  - **MDE** exhibits the most stable grading profile, with consistently high A–B shares and low failure rates.
  - **PED** and **BS** show moderate stability with limited variation over time.
  - **ENG** and **LAW** display greater volatility in grade composition and more pronounced changes in failure outcomes.
- Engineering courses consistently show lower high-grade shares and higher failure rates relative to other departments, though they also exhibit a stronger decline in failures in later semesters.

---

## Interpretation & Implications

The results suggest that changes in academic outcomes following the introduction of LLMs are gradual rather than abrupt and are not uniform across disciplines. Aggregate trends mask meaningful department-level dynamics, highlighting the importance of disaggregated analysis when evaluating the impact of emerging educational technologies.

Given the descriptive nature of the study, findings should be interpreted as observed patterns rather than evidence of causal effects.

---

## Limitations

- The analysis is observational and does not establish causality.
- Potential confounding factors (e.g., curriculum changes, assessment policies, cohort composition) are not explicitly controlled.
- Publicly available datasets are anonymized and aggregated, limiting individual-level analysis.
- Results reflect the institutional context of a single university and may not generalize universally.

---

## Repository Structure

.
├── LLM_Impact.ipynb     # Full analytical workflow, EDA, and visualizations
└── data/
    └── raw/             # Anonymized, pre-processing datasets used in the analysis

All data wrangling, aggregation, and analysis steps are documented and executed within the notebook.

---

## Author & Context

**Author:** Nurmukhamed Absattarov  
**Institution:** SDU University  

This project was conducted as an individual university research project under the supervision of  
**Bakhtiyor Meraliyev**, Senior Lecturer and Information Systems Educational Program Coordinator,  
SDU Faculty of Engineering and Natural Sciences.

The repository is included as part of an academic analytics portfolio.
