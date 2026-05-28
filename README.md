# Income Inequality Analysis - Europe 2022

Analysis of income inequality across European countries using Eurostat earnings data and World Happiness Report metrics.

## Overview

This project examines the relationship between income inequality (measured as the percentage gap between mean and median earnings) and national happiness scores across 34 European countries in 2022.

<img src="salary and happiness.png" alt="Salary and Happiness">

## Data Sources

* **Eurostat**: Mean and median gross hourly earnings data (2022)
  * Sector: All NACE activities except public administration (B-S_X_O)
  * File: `eurostat_mean-median_2026.csv`
* **World Happiness Report 2022**: National happiness scores synchronized with earnings data year

## Key Findings

* **Highest inequality**: Bulgaria (26.55%), Albania (26.05%), Portugal (25.61%)
* **Lowest inequality**: Denmark (1.46%), Norway (4.08%), Iceland (4.95%)
* **Poland**: 18.37% inequality (10th highest), happiness score 6.125
* **European average**: 15.36% inequality
* **Correlation**: Pearson coefficient (r) calculated between inequality and happiness

## Visualizations

1. **Horizontal bar chart** with Poland highlighted in red and European average line
2. **Dark-themed premium chart** with country labels in Polish
3. **Interactive dashboard** with normalized comparison of inequality vs. happiness

## Technical Stack

* **PySpark**: Data processing and transformation
* **Matplotlib**: Static visualizations
* **Databricks AI/BI Dashboard**: Interactive analytics
* **Unity Catalog**: Data storage and management

## Methodology

**Income Inequality Calculation:**
```
Inequality (%) = ((Mean - Median) / Mean) × 100
```


**Normalization:**
* Min-Max normalization (0-1 and 0-100 scales)
* Enables visual comparison of inequality and happiness on the same scale

## Files

* `Notebook.ipynb` - Main analysis notebook
* `eurostat_mean-median_2026.csv` - Source data
* Dashboard: "Income Inequality Analysis - Europe 2022"

## Usage

1. Run Cell 1 to load and process Eurostat data
2. Run Cell 2-3 for inequality visualizations
3. Run Cell 4 to add happiness scores and calculate correlation
4. Open dashboard for interactive exploration with normalized metrics

## Author

Szczerski using Databricks

---

*Data reflects 2022 earnings and happiness metrics. Excludes eurozone aggregates (EA19, EA20, EU27_2020).*
