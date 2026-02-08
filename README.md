# House-Price-Prediction-XGBoost
## 📌 Overview
This project is an end-to-end Machine Learning pipeline designed to predict residential housing prices. Using the Ames Housing dataset (80 features), I built a model that estimates sale prices with an error rate (RMSLE) of **0.135**, placing it competitively on the Kaggle leaderboard.

## 🛠️ Tech Stack
* **Python** (Pandas, NumPy)
* **Machine Learning:** XGBoost (Gradient Boosting), Scikit-Learn
* **Preprocessing:** One-Hot Encoding, SimpleImputer (Mean/Most Frequent)
* **Feature Engineering:** Domain-specific feature creation (Total Square Footage)

## 🚀 Key Strategy
The model improvement relied on three core pillars:
1.  **Smart Imputation:** Differentiated strategies for numerical (mean) vs. categorical (mode) missing data.
2.  **Feature Engineering:** Created a `TotalSF` (Total Square Footage) feature by combining basement, 1st, and 2nd-floor areas, which significantly increased model correlation with price.
3.  **Hyperparameter Tuning:** Tuned XGBoost with `n_estimators=1000` and `learning_rate=0.03` to prevent overfitting while maximizing pattern recognition.

## 📊 Results
* **Base Model Score:** 0.13824
* **Engineered Model Score:** 0.13596

* Built by Ankur Singh as part of a Data Science portfolio project
