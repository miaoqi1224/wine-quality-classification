# Diamond Price Regression Analysis

A multi-part regression analysis of diamond pricing — from descriptive statistics to multiple linear regression with diagnostics.

## Overview

Using a 2022 diamond prices dataset, this project walks through the full regression workflow: sampling, exploratory analysis, correlation structure, model fitting, and interpretation. Built as PSTAT 126 (Regression Analysis) coursework at UC Santa Barbara.

## What's inside

- **Part 1 — Data description & descriptive statistics**: random sampling, variable typing, summary statistics, correlation matrix with scatterplots, boxplots of price by cut/color
- **Part 2** — extended modeling and inference
- **Part 3** — model refinement and conclusions
- **Full project report** (`126project`) — end-to-end write-up

Core techniques: multiple linear regression (`lm`), correlation analysis, residual diagnostics, categorical predictor handling (cut, color, clarity).

## Files

- `126project.Rmd` / `126project.pdf` — complete project report (source + rendered)
- `126part2.Rmd` / `126part2.pdf`, `126part3.Rmd` / `126part3.pdf` — staged analysis parts
- `Diamonds_Prices2022.csv` — dataset

## Run it

```r
# Requires: dplyr, ggplot2
rmarkdown::render("126project.Rmd")
```

## Author

Miao Qi — M.A. Statistics, Columbia University (Advanced Machine Learning Track).
