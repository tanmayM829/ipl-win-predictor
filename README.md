# IPL Win Predictor

## Overview
A Machine Learning project predicting IPL matches outcomes using pre-match featuers.
Build using python, pandas, scikit learn and matplotlib

## Key Finding
Initially the model achieved an accuracy of 85%, however that was due to data leakage - post-match columns (result_margin, target_runs etc) were included in the features.

After removing leaky features, the accuracy plummeted to roughly 50%, revealing that pre-match information (teams, venue, toss) alone has limited predictive power.

## Tech Stack
- Python, Numpy, Pandas
- Scikit-learn (Logistic Regression, KNN, Decision Tree, Random Forest, SVM)
- Matplotlib, seaborn

## Models Compared

Model   &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;     Train  &emsp;   Test

Logistic Regression     &emsp;     0.530  &emsp;  0.491\
KNN &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;  0.672  &emsp;  0.486\
Decision Tree     &emsp;&emsp;&emsp;&emsp;  0.559  &emsp;  0.491\
Random Forest     &emsp;&emsp;&emsp;&nbsp;       0.853  &emsp;  0.468\
SVM &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;    0.702  &emsp;  0.495


## The Things which may improve it
- Historical win rates per team
- Head to head records
- venue specific win rates
- Player availibility data

## Dataset
IPL Dataset 2008-2024 from Kaggle
