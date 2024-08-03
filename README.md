# Predicting Future U.S. Elections Using Pre-2020 Survey Data

**Project Overview**

This project aims to predict the outcomes of future U.S. elections by analyzing pre-2020 survey data. The analysis explores various predictive features, model performance metrics, and insights derived from machine learning models trained on the dataset. It also includes an AI-powered political candidate comparison feature to enhance the decision-making process for voters.

**Data Preprocessing and Feature Engineering**

**Steps:**
- Data Cleaning: Addressed null values, converted date columns, and summarized numeric feature distributions.
- Descriptive Analysis: Examined candidate distribution across states and nationally.
- Data Exploration: Visualized state-level and national-level poll winners, calculated means of key features.

**Feature Engineering:**
- Derived new features: adjustment_impact, house_effect, trend_effect, and poll_to_poll_change.
- One-hot encoded categorical features.
- Created a target variable poll_winner.
- Engineered a high_electoral_votes feature indicating states with high electoral votes.

Data Preparation: Split and merged datasets, renamed columns, and addressed multicollinearity.

# **Model Development**

**Techniques:**
- Data Splitting: Used stratified fold method, with a 70-30 training-test split.
- Model Training: Trained RandomForestClassifier and XGBoostClassifier using cross-validation, L1 regularization, and GridSearchCV for parameter optimization.
- Model Evaluation: Evaluated models using F1 score, Recall, Precision, Accuracy, confusion matrix, and ROC curve.

# **Findings**
General Observations:
- Biden led in a majority of the polls and states with high electoral votes.
- Models indicated the importance of house effects and public perception on election outcomes.

**Model Performance:**
- RandomForestClassifier: F1 Score: 0.939, Recall: 0.985, Precision: 0.897, Accuracy: 0.899.
- XGBoostClassifier: F1 Score: 0.94, Recall: 0.987, Precision: 0.897, Accuracy: 0.90.
- Both models performed similarly, with XGBoost having a slight edge in recall and accuracy.

**Insights:**
- House effects and public perception were significant in predicting election outcomes.
- High electoral vote states played a crucial role in predictions.
- XGBoost generalized better on the test set.

# AI-Powered Political Candidate Comparison Feature

**AI Models and Techniques:**
- NLP: Analyzes candidate speeches and public statements for sentiment, tone, and policy preferences.
- Recommendation System: Matches voter preferences with candidates’ political outlooks.
- Cloud ML Feature Design: Implements computations in the cloud for real-time predictions.

**Live Data Feeds Integration:**
- API Integration: Incorporates live data from reputable sources.
- Real-time Sentiment Analysis: Monitors social media and news outlets continuously.
- User Feedback Loop: Incorporates user feedback for model optimization.

**Challenges**
- Limited dataset size for robust model training.
- Incomplete data descriptions, requiring additional research.
- Time constraints in model development.
