# LHL_Final_Project - NBA Draft Predictor

## Project/Goals
The goal of this project is to leverage machine learning skills to predict the results of an NBA draft.  

## Process
Step 1: Acquired a dataset that contained advanced and standard stats for all college basketball players between 2009 and 2021. 

Step 2: Performed exploratory data analysis and feature engineering.

- Identified different trends amongst drafted vs undrafted players and accounted for class imbalances. 

Step 3: Prepare Baseline model performances to select the right model. 

- Built pipelines to evaluate 5 different regression model techniques. 

Step 4: Perform model tuning to optimize results.
- Leveraged gridsearch on an XgBoost pipeline with kfold cross validation. 

## Results
An xgboost model was chosed for tuning and came within 13 MSE which can provide a good range for a player's potential draft position. However as a draft progresses to later first round into the second round, the available players become harder to differentiate and teams begin to select based their individual needs rather than stats. 

## Challenges:

- Since the dataset consisted of college players, there was missing draft results for european players.
- Duplicate draft results i.e. when a player was in college for multiple years, their draft result was duplicated across their rookie to senior years. Addressed this issue by grouping by best year. 


## Future Goals
Would like to incorporate more nba team related data to build in a team's needs aspect into the algorithm since a team may not always try to draft the best statistical player available.
