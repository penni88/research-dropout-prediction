# Predicting Participant Dropout in Longitudinal Research Studies

## Overview
Participant dropout is one of the most costly challenges in longitudinal research. 
This project uses simulated data modeled on realistic lab conditions to explore 
whether intake-level variables can predict which participants are most at risk 
of dropping out before it happens.

## Background
During two years as a research assistant, I observed firsthand how dropout 
disrupted longitudinal studies. This project applies data analysis to a problem 
I watched play out in real time.

## Dataset
Simulated dataset of 200 participants with the following features:
- Age
- Commute distance (miles)
- Session length (60 vs 120 minutes)
- Sessions completed (1, 2, or 3)
- Employment status (employed, unemployed, student)

Overall dropout rate: 38.5%

## Model
Logistic regression trained on 80% of data, tested on held-out 20%.

**Results:**
- Accuracy: 75%
- Dropout Precision: 93%
- Dropout Recall: 61%
- F1-score: 0.75

## Key Finding
Sessions completed was the strongest predictor of dropout (importance: 1.104), 
followed by employment status (0.381). Unemployed and student participants 
dropped out at higher rates than employed participants, consistent with 
published retention literature.

## Tools
Python, pandas, numpy, scikit-learn, matplotlib, seaborn

## Files
- `dropout_prediction.ipynb` — full analysis notebook
- `dropout_exploration.png` — exploratory charts
- `feature_importance.png` — feature importance visualization
