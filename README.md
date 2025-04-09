📊 Project Overview
This notebook project includes:
1. Exploratory Data Analysis (EDA):
  Loaded and cleaned football team and match statistics from Kaggle.
  Merged home and away team stats with game results.
  Engineered new features such as:
    Goal difference
    Shots, xGoals, fouls, and possession-based metrics (e.g., PPDA)
    Win indicators
  Visualized trends using descriptive statistics and feature correlations.
2.Feature Engineering:
  Created aggregated features: average goals, shots, PPDA per team.
  Mapped bookmaker odds for home and away teams.
  Used team-level historical data to estimate performance strength.
3. Machine Learning Models:
  Classification (XGBoost): Predict whether the home team will win.
  Regression (XGBoost): Predict expected goals for both home and away teams.
  Evaluated with metrics like accuracy (for classification) and RMSE (for regression).
4. Match Outcome & Score Prediction:
  Custom function to simulate a future match between any two teams.
  Accepts team names and returns the predicted score and winner.

🧠 ML Models Used
XGBClassifier: Binary classification for predicting home win.

XGBRegressor: Two regressors to predict goals scored by each team.

Models trained using game-level features engineered from team stats.

🗂️ Files
Football_analysis.ipynb: Full notebook with EDA, preprocessing, modeling, and prediction.

🚀 Future Improvements
Deploy the prediction function using Flask or FastAPI as a web app.
Add interactive dashboards using Streamlit or Dash.
Improve feature extraction (e.g., add form/streak, recent performance).
Include season-wise trends or league-level differences.

📌 Data Source
https://www.kaggle.com/datasets/technika148/football-database/data?select=appearances.csv
