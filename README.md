# Housing Price Index Forecasting

A team project comparing traditional time-series and machine-learning approaches for forecasting the **New Taipei City Housing Price Index**.

> **Project type:** Team project  
> **Methods compared:** VAR, SVR, LSTM  
> **Evaluation metric:** MAPE

## Overview

This project examined whether machine-learning approaches could improve housing price index forecasts relative to a traditional multivariate time-series benchmark.

The study period covered **January 2013 to December 2022** and focused on the New Taipei City housing market.

## Target Variable

- **Housing Price Index (HI)**

## Candidate Predictors

The project considered housing-market and macroeconomic indicators such as:

- Housing Price-to-Income Ratio (PIR)
- Five major banks' new mortgage loans (HR)
- New housing mortgage burden ratio (REER)
- Foreign Direct Investment (FDI)
- Construction-related price / activity indicators
- Taiwan Weighted Stock Index (TWII)
- Consumer Price Index (CPI)
- Housing transaction volume

## Methods

### VAR
Vector Autoregression served as the traditional multivariate time-series benchmark.

### SVR
Support Vector Regression was used as a nonlinear machine-learning forecasting approach.

### LSTM
Long Short-Term Memory networks were used to model sequential patterns in the time series.

## Workflow

1. Data transformation and preprocessing
2. Time-window construction
3. Model training
4. Forecasting
5. Model comparison using MAPE

## Results

The project poster reports the following MAPE results.

### Longer-horizon comparison

| Model | M1 | M2 | M3 |
|---|---:|---:|---:|
| VAR | 2.33% | 2.43% | 1.53% |
| SVR | 3.59% | 3.37% | 0.65% |
| LSTM | 2.02% | 1.85% | 0.60% |

### One-quarter-ahead comparison

| Model | M1 | M2 | M3 |
|---|---:|---:|---:|
| VAR | 0.22% | 0.59% | 0.87% |
| SVR | 0.68% | 0.88% | 0.46% |
| LSTM | 0.78% | 0.82% | 0.64% |

The project conclusion indicates that traditional time-series modeling remained strong for short-horizon forecasting, while machine-learning models were competitive for longer-horizon prediction under the tested settings.

## My Contribution

The available project poster identifies this as a team project but does not document the responsibility of each member.

This repository therefore **does not attribute the complete modeling workflow to me individually**. My exact contribution will be added once the team responsibilities are documented.

## Repository Structure

```text
housing-price-forecasting/
├── README.md
├── data/
│   └── README.md
├── src/
│   └── README.md
├── results/
│   └── model_comparison.csv
├── figures/
│   └── README.md
├── report/
│   └── README.md
└── .gitignore
```

## Source Code Status

The original modeling scripts were not included in the files currently available for this portfolio build, so this repository does not fabricate or recreate them.

When the original VAR / SVR / LSTM code is available, it can be added under `src/` and linked to the exact experiments shown in the poster.

## Project Materials

The project poster is available through my Notion portfolio:

[Data Analytics & Science Portfolio](https://app.notion.com/p/Data-Analytics-Science-Portfolio-160bcf9053b6800198faddd8f6e6a8ab)

## Tools & Topics

- Time Series
- VAR
- Support Vector Regression
- LSTM
- Forecasting
- MAPE
- Model Comparison

---
Portfolio repository maintained by **Yi-Ling Dai**.
