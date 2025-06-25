NBA Game Outcome Prediction

By: Vidushi Gupta, Jeffrey Oduman, Darian Parks

---

Overview

This project analyzes historical NBA game data to predict the outcome (win/loss) of games using machine learning models. We used rolling averages to predict the win/loss outcome for the next game based on the past 5 games.

---

Methodology

* Feature Engineering

* Calculated 5-game rolling averages for stats like field goals, assists, rebounds, turnovers, etc., to simulate real-world prediction without data leakage.
* Derived new metrics like possessions, offensive efficiency, and scoring breakdowns to understand evolving team strategies over time.

* Exploratory Data Analysis (EDA)

* Visualized missing data and filtered out unreliable features.
* Analyzed correlations to determine the most predictive features (e.g. field goal %, free throws).
* Examined offensive vs. defensive trends and the rise of 3-point shooting over decades.

Machine Learning Models

We evaluated three models to predict whether the home team wins:

* Random Forest: 90% accuracy with strong interpretability.
* XGBoost: 97% accuracy after hyperparameter tuning; best-performing model.
* Logistic Regression: 85% accuracy with valuable coefficient insights.

---

Key Results

* Top Predictors: Field goal percentage (both teams), free throws made, and turnovers.
* Model Evaluation: XGBoost achieved the highest precision, recall, and AUC (0.93+).
* Hyperparameter Tuning: Used `Optuna` and `BayesSearchCV` for Random Forest and XGBoost for performance improvement.

---

Technologies Used

* Python (pandas, numpy, scikit-learn, xgboost, optuna)
* Jupyter Notebook
* Plotly & Seaborn for visualizations
* Kaggle for dataset sourcing
