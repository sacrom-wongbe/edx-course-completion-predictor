# **edX Course Completion Predictor**

A machine learning system that predicts online learner course completion using de-identified HarvardX/MITx edX performance data. This project focuses on building **interpretable, industry-standard predictive models** to support student success analytics, retention forecasting, and early-warning systems.

## **📌 Overview**

The rise of massive open online courses (MOOCs) has created vast datasets but also extremely high dropout rates. This project explores whether student engagement and activity patterns can reliably predict course completion.

Instead of reaching for neural networks, the goal here is to demonstrate **how classic, production-friendly models can deliver high performance with transparency**, faster iteration cycles, and simpler deployment paths.

The final Random Forest model achieves **97.26% accuracy**, outperforming baseline logistic regression and offering strong feature-level interpretability.

---

## **🎯 Objectives**

* Build a reliable, lightweight ML pipeline for predicting MOOC completion.
* Prioritize **interpretability**, **speed**, and **industry alignment** over heavyweight deep learning models.
* Engineer meaningful behavioral features derived from temporal engagement patterns.
* Create a Kaggle-ready inference pipeline for reproducible evaluation.

---

## **🧠 Machine Learning Approach**

### **Models Implemented**

* **Logistic Regression**
  Useful as a transparent, linear baseline; establishes initial feature importance signals.
* **Random Forest Classifier** *(Best: 97.26% accuracy)*
  Provides strong non-linear decision boundaries and robust performance without heavy tuning.

### **Why Not Neural Networks?**

* Classic tabular ML models:

  * Train faster
  * Require fewer hyperparameters
  * Offer easier interpretation
  * Are widely deployed in education analytics, HR, finance, and healthcare
* This aligns with industry practice for **fast-turnaround prediction problems on structured data**.

---

## **📊 Feature Engineering**

### **Features Used**

* **Engagement Metrics:**
  `events`, `active_days`, `videos_watched`
* **Course Context:**
  `course_id`, `certification track`, demographic indicators
* **Time-Based Features:**

  * **`duration_days`** – engineered as the total span of learner activity
  * Helps model pacing, consistency, and dropout risk

### **Feature Importance**

The Random Forest model highlights engagement intensity and consistency as dominant predictors.

---

## **🛠️ Tools & Tech Stack**

* **Python**
* **pandas, NumPy**
* **scikit-learn** (modeling, evaluation)
* **matplotlib & seaborn** (exploratory data analysis + visuals)
* **Jupyter Notebook** (experiment execution + documentation)
* **Kaggle** leaderboard submission pipeline

---

## **📈 Usage**

The notebook includes:

1. Data cleaning + preprocessing
2. Feature engineering
3. Train/test model pipeline
4. Hyperparameter tuning for Random Forest
5. Evaluation metrics (accuracy, confusion matrix, ROC curve)
6. Kaggle-ready CSV export

To run locally:

```bash
pip install -r requirements.txt
jupyter notebook
```

---

---

## **🚀 Potential Extensions**

* Early-warning intervention system for at-risk students
* Gradient boosting models (XGBoost / LightGBM)
* Survival analysis for dropout timing
* Real-time integration with LMS event streams
* Explainability reports (SHAP, LIME)

---
