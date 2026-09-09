# Displaced Population Data Analysis

Data cleaning, feature engineering, and exploratory analysis on a humanitarian dataset tracking housing and demographic conditions across displaced population sites in Iraq, Libya, Syria, and Yemen (Jan 2017 – Nov 2018).

## Overview

The raw dataset (9,917 records) had structurally missing housing-type data and no derived features for comparing countries or housing conditions. This project cleans the data, engineers new features, and analyzes population and housing patterns across countries and time.

## Objectives

- Diagnose and correctly handle structural missing values in the housing columns
- Engineer features that describe gender balance, housing density, and dominant housing type per site
- Compare population and housing patterns across countries and over time
- Identify relationships between housing type and site characteristics

## Dataset

- 9,917 records across Iraq, Libya, Syria, and Yemen
- Columns include identification, population counts (Members, gender split), and housing-type counts (Room, Flat, House, Tent)
- Time range: January 2017 – November 2018

## Tools & Technologies

Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

## Methodology

- Structural diagnostics (`df.info()`, `df.describe()`) to profile raw columns
- Root-cause analysis of missing values in housing columns, followed by domain-informed imputation (0, not a statistical placeholder)
- Date parsing and derivation of year/month/day fields
- Categorical text cleaning to prevent duplicate labels
- Feature engineering: gender ratio, people-per-house density, dominant housing type
- Grouping/pivoting by country and country × year
- Min-Max scaling, Z-score standardization, and outlier detection (|Z| > 3)
- Multi-panel visualization and correlation analysis

## Key Insights

- Yemen (~24.0M cumulative Members) and Syria (~19.5M) form a clearly higher population tier than Iraq (~7.9M) and Libya (~7.7M)
- Room, Flat, and House correlate near-perfectly with each other (r ≈ 1.00), while Tent correlates strongly negatively with all three (r ≈ -0.90) — sites are effectively either tent-based or conventional-housing-based, rarely both
- All four countries show a mild decline in recorded population between 2017 and 2018
- No records exceeded the 3-sigma outlier threshold despite Members ranging from 5 to nearly 16,000

## Results / Outcome

The pipeline brought the dataset to 100% completeness using domain-informed imputation and produced engineered features and visualizations clarifying which countries and housing types dominate the recorded displacement data.

## Project Structure

```
displaced-population-analysis/
│
├── README.md
├── data/
├── notebooks/
├── src/
├── outputs/
└── requirements.txt
```

## Skills Demonstrated

Data Cleaning, Feature Engineering, Exploratory Data Analysis, Data Aggregation & Pivoting, Feature Scaling, Outlier Detection, Data Visualization
