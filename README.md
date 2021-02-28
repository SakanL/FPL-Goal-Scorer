# FPL-Goal-Scorer
Multi algorithm machine learning to predict English Premier League goal scorer

1. Introduction
Premier league football is the professional football (soccer) competition in United Kingdom, one of the most popular sport events in the world. Fantasy Premier League is a game that casts you in the role of a Fantasy manager of Premier League. You are given the task to pick a squad of real-life players who score points for your team based on their performances in their own matches. As in 2020 there are 7,367,252 people joined this game. Our target in this project is to predict performance of the player in next match.

2. Approach
Fantasy Premier League (FPL) provide API to retrieve data as json format, we will download the data to local machine and working on it. We will use machine learning workflow to define the best model.


3. Dataset and Metric
From all information, we will focus only on 2 datasets, team data and player data, then we will merge these together. Team data contains 22 columns while Player data contains 20 columns. After merged we will have 12 columns as the following:
Assists 
Bps 
goals_scored 
opponent_team
o_team
strength
strength_overall_home
strength_overall_away
strength_attack_home
strength_attack_away
strength_defence_home
strength_defence_away

The strength_xx will be predictors for goals_scored to predict if the player can score in a match or not.

4. Results
We have explored the data and found a little correlation between variables, as a result Linear regression model cannot get the satisfied result, only score 0.1 on accuracy. Then we move to ANN and this time we have got accuracy score at 0.9 Finally we use SVM and the accuracy of training is better than ANN.
Since we have small data set, in the project we will choose SVM as our model to predict the goals scored by soccer player.


