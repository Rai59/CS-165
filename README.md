# Forest Fire Prediction — Algeria

A machine learning project to predict forest fire occurrence using meteorological data and fire weather indices.

## Overview

This project develops a binary classification system to predict whether a forest fire will occur based on weather conditions. Three models are compared — Logistic Regression, k-Nearest Neighbours, and Random Forest — with Random Forest achieving the best performance at **95.9% accuracy**.

## Dataset
- **Size:** 243 observations from two Algerian regions (Bejaia and Sidi-Bel Abbes)
- **Period:** June – September (fire season)
- **Features:** Temperature, humidity, wind speed, rainfall, and Fire Weather Index components (FFMC, DMC, DC, ISI, BUI, FWI)

## Results

| Model | CV Accuracy | Test Accuracy |
|-------|-------------|---------------|
| Logistic Regression | 92.8% | 93.9% |
| k-Nearest Neighbours | 87.6% | 93.9% |
| Random Forest | 97.4% | 95.9% |

## Key Findings

- **FWI and Drought Code (DC)** are the strongest predictors — sustained fuel moisture depletion matters more than single-day weather
- **August** has the highest fire occurrence; **June** the lowest
- Random Forest outperforms linear models by capturing non-linear feature interactions

## Tech Stack

- Python 3
- pandas, NumPy
- scikit-learn
- Matplotlib, Seaborn
- 
## Future Improvements

- Hyperparameter tuning (GridSearchCV)
- Time-based cross-validation for realistic evaluation
- Add region as a categorical feature
- Deploy as a real-time risk scoring API

## Author

Rai — Computer Science, Swansea University
