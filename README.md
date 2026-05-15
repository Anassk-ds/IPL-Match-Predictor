# IPL Match Outcome Predictor 🏏🤖

## 📌 Project Overview
This repository contains a Machine Learning classification project designed to predict the winning probability of an IPL match based on live game situations. By analyzing variables like current score, target, wickets dropped, and balls remaining, the model calculates real-time win/loss percentages for the batting and bowling teams.

## 📊 Key Features & Logic
* **Feature Engineering:** Structured live match scenarios using situational features such as runs needed, balls left, wickets remaining, and total target.
* **Data Preprocessing:** Implemented Label Encoding via `scikit-learn` to transform categorical text data (team names and venues) into numerical values optimized for model training.
* **Predictive Modeling:** Trained a **Random Forest Classifier** to evaluate high-pressure match scenarios and classify outcomes.
* **Live Predictor Function:** Created a custom execution function that takes any real-time match situation input and outputs a precise probability breakdown (e.g., KKR: 65% chance of winning, CSK: 35%).

## 🛠️ Tech Stack & Tools
* **Language:** Python
* **Machine Learning Library:** Scikit-Learn
* **Data Libraries:** Pandas, NumPy
* **Environment:** Google Colab / Jupyter Notebook

## 🚀 How It Works (Sample Code Input)
You can test custom scenarios directly within the model notebook using the deployed function:

```python
predict_winner(batting_team='KKR', bowling_team='CSK', venue='Kolkata', 
               runs_needed=12, wickets_left=8, balls_left=6, target=145)
