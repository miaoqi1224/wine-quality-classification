# White Wine Quality Classification

A comparative study of machine learning techniques for classifying white wine quality from physicochemical properties.

## Overview

Using the Wine Quality dataset (4,898 white wine samples, 11 chemical features), this project frames wine quality as a three-class classification problem — **inferior**, **ordinary**, and **superior** — and compares three classifiers: **k-Nearest Neighbors**, **Decision Tree**, and **Random Forest**.

## Key Results

| Model | Test Accuracy |
|---|---|
| Random Forest | **94.08%** |
| k-NN | >92% |
| Decision Tree | >92% |

Random Forest emerged as the top performer. Analysis also surfaced meaningful feature relationships (e.g., density vs. residual sugar) and the challenge of class imbalance — both inferior and superior wines proved harder to classify than ordinary ones.

## Methodology

1. **Exploratory data analysis** — distributions, correlations (`corrplot`), identification of redundant features
2. **Feature selection** — removed near-zero-variance and highly correlated features to reduce redundancy
3. **Model training** — 10-fold cross-validated k-NN, Decision Tree (`rpart`), and Random Forest (`randomForest`)
4. **Evaluation** — confusion matrices, per-class accuracy, feature importance

## Files

- `131-final.Rmd` — full analysis source (R Markdown)
- `131-final.pdf` — rendered report
- `winequality-white.csv` — dataset (semicolon-delimited)

## Run it

```r
# Requires: readr, dplyr, ggplot2, corrplot, caret, rpart, randomForest, e1071
rmarkdown::render("131-final.Rmd")
```

## Author

Miao Qi — M.A. Statistics, Columbia University (Advanced Machine Learning Track). Originally developed as the PSTAT 131 final project at UC Santa Barbara (with Wei Xie).
