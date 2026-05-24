# Playdale Quote Insights

A machine learning and analytics project focused on understanding the factors influencing quote-to-order conversion in B2B sales environments.

This project was completed as part of an industry dissertation placement with Playdale Playgrounds Ltd.

---

## Business Problem

In B2B sales environments, companies generate large volumes of quotations, but not all convert into successful orders.

Understanding the factors associated with successful quote conversion can improve:
- sales prioritisation
- quotation strategies
- regional targeting
- product recommendations
- operational efficiency

This project investigates which factors are most strongly associated with successful quote conversion using statistical and machine learning techniques.

---

## Objectives

- Clean and standardise raw quotation datasets
- Prevent data leakage by restricting features to quote-creation-time information
- Identify key drivers of successful quote conversion
- Compare interpretable and non-linear machine learning models
- Analyse regional and client-specific product success patterns

---

## Methodology

This project followed a leak-aware and reproducible machine learning workflow designed for real-world B2B sales analytics.

### Data Preparation

The raw quotation datasets required extensive preprocessing, including:
- identifier consolidation
- quote deduplication
- geographic standardisation
- status harmonisation
- missing value handling

Only information available at the time of quote creation was retained to prevent data leakage.

### Feature Engineering

Features were engineered from:
- client/company type
- geographic region
- country
- quote creation timestamp
- month, quarter, and day-of-week seasonality indicators

### Machine Learning Models

The following models were evaluated:
- Logistic Regression
- Random Forest
- Gradient Boosting

Logistic Regression was used as an interpretable baseline model, while Random Forest served as a non-linear ensemble benchmark capable of capturing more complex interactions.

### Evaluation Metrics

Models were evaluated using:
- ROC-AUC
- Recall
- F1-score
- Precision-Recall analysis

Special attention was given to recall for successful quote conversions to minimise missed opportunities.

### Product-Line Analysis

A supplementary won-only product analysis was performed to identify:
- high-performing product groups
- regional product preferences
- client-specific product patterns

This provided actionable business insights beyond predictive modelling alone.

---

## Workflow

![Workflow](images/workflow.png)

---

## ROC Curve

![ROC Curve](images/roc_curve.png)

---

## Feature Importance

![Feature Importance](images/feature_importance.png)

---

## Key Findings

- Geography and client type were the strongest predictors of quote conversion.
- Random Forest achieved the strongest predictive performance.
- Seasonal patterns influenced conversion behaviour.
- Product success patterns varied significantly across regions and client types.
- A relatively small subset of products accounted for a large proportion of successful quotes.

---

## Technologies Used

- Python
- pandas
- NumPy
- scikit-learn
- Matplotlib
- Jupyter Notebook

---

## Repository Structure

```text
playdale-quote-insights/
│
├── README.md
├── dissertation_report.pdf
├── images/
│   ├── workflow.png
│   ├── roc_curve.png
│   └── feature_importance.png
```

---

## Confidentiality Notice

Due to company confidentiality agreements, the original datasets and source code used in this project cannot be publicly shared.

This repository contains:
- project overview
- methodology
- selected visualisations
- findings
- dissertation report

No confidential business data has been included.

---

## Future Work

Potential future enhancements include:
- richer calendar-based features
- quote recommendation systems
- real-time dashboards
- product bundle recommendation systems
- advanced ensemble modelling

---

## Dissertation Report

The full dissertation report is included in this repository.
