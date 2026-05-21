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
- `PT Retention.ipynb` — full analysis notebook
- `Exploratory_Graph.png` — exploratory charts
- `Feature_Importance_Graph.png` — feature importance visualization

## References
- Glomstad, M., Sorby, I. D., Holt, T., & Bjørkly, S. (2023). Client predictors of therapy dropout in a primary care setting: A prospective cohort study. *BMC Psychiatry*. https://pmc.ncbi.nlm.nih.gov/articles/PMC10207790/
- Gustavson, K., Røysamb, E., von Soest, T., Mathiesen, K. S., & Karevold, E. (2012). Attrition and generalizability in longitudinal studies. *BMC Research Notes*. https://doi.org/10.1186/1756-0500-5-1
- Melanie McGovern, Joar Øveraas Halvorsen, Marte Svarver Ørstavik, Bård Dyrdal, & Stål Bjørkly. (2024). Who will stay and who will go? Identifying risk factors for psychotherapy dropout. *Counselling and Psychotherapy Research*. https://doi.org/10.1002/capr.12783
- Ribisl, K. M., Walton, M. A., Mowbray, C. T., Luke, D. A., Davidson, W. S., & Bootsmiller, B. J. (1996). Minimizing participant attrition in panel studies through the use of effective retention and tracking strategies: Review and recommendations. *Evaluation and Program Planning, 19*(1), 1–25.
- Swift, J. K., & Greenberg, R. P. (2012). Premature discontinuation in adult psychotherapy: A meta-analysis. *Journal of Consulting and Clinical Psychology, 80*(4), 547–559. https://doi.org/10.1037/a0028226
