# edX Course Completion Predictor

This project builds a machine learning model to predict whether students will complete online courses on the edX platform, using de-identified data from HarvardX and MITx.

## Models Used
- Logistic Regression
- Random Forest Classifier (best: 97.26% accuracy)

## Features
- Student engagement metrics (e.g., events, active days, videos watched)
- Demographics and course info
- Engineered time-based feature: `duration_days`

## Tools
- Python, pandas, scikit-learn, Jupyter Notebook
- Visualizations with matplotlib and seaborn

## Usage
Model predictions are submitted to a Kaggle leaderboard for evaluation. This notebook includes preprocessing, model training, evaluation, and Kaggle-ready CSV export.

