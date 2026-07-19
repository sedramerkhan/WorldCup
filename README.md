# FIFA World Cup Data Engineering & Insights Pipeline

This repository contains a Jupyter Notebook focused on cleaning, consolidating, and extracting historical insights from disjointed FIFA World Cup datasets (matches, stadiums, attendance, and squads).

## Overview
The project is split into two core phases:
1. **Data Engineering:** Aligning disjointed tables, resolving structural name discrepancies for historical geopolitical entities, and correcting flipped home/away match contexts.
2. **Exploratory Data Analysis (EDA):** Extracting historical trends regarding team performance, crowd dynamics, and squad demographics.

## Analytical Insights Extracted
* **Home-Field Advantage Analysis:** Evaluated the statistical impact of crowd size and host-nation status on match outcomes and scoring margins.
* **Geopolitical Trend Tracking:** Visualized the historical shifts in global football dominance, tracking performance before and after the restructuring of historical states.
* **Squad Demographics & Success:** Correlated squad age distributions and player experience metrics against tournament progression.

## Data Pipelines & Cleaning Steps
* **Attendance & Context Corrections**: Standardized historical country variations (e.g., `West Germany` $\rightarrow$ `Germany`) to fix indexing errors, and resolved flipped home/away records using dynamic date-matching criteria.
* **Squad Linkages**: Programmatically mapped international team codes (`team_code`) and structural IDs across over 8,400 global player profiles using custom text-unification functions.
* **Integrity Validation**: Enforced zero-tolerance assertion steps (`check_all_na`) and strict shape checks post-merge to prevent data loss.

## Required Dependencies
```bash
pip numpy pandas plotly scipy scikit-learn
