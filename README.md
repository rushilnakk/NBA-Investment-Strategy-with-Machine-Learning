# NBA-Investment-Strategy-with-Machine-Learning
Performed binary classification of NBA players to predict future Hall of Fame inductees for a memorabilia investment strategy in Python.

# Business Problem
In this project I used real data on past basketball players to develop a machine learning model to inform memorabilia investment decisions. The dataset includes 27 different predictors/attributes on each player, with the target variable indicating whether or not the player has been inducted into the Hall of Fame. The task was to build a classification model predicting whether or not a player will be inducted and to apply this model to select players to invest in. The goal is to develop a strategy that maximizes profitability while investing $4,000,000 in the memorabilia of up to 100 players. The revenue from selling the memorabilia of an inducted player is estimated to be $120,000, while a non-inducted player results in a loss of 50% of the initial investment.

# Approach
Since the data collection process was complete in this project, my biggest challenge was to identify the key feautures which are important to predict whether an NBA player will be inducted to the Hall of Fame or not. I first cleaned my data to remove redundant and insignificant predictors using a wrapper function I created as well as **Recursive Feature Elimination**. I then proceeded with my analysis by training and comparing the following machine learning algorithms using the **sci-kit learn** library in Python:
1. Decision Tree
2. Random Forest
3. Bagging
4. Naive Bayes
5. K-nearest Neighbors

Following the creation of these models, their performances were evaluated by testing accuracy and area under the ROC curve. The best model was then used to estimate profitability using testing data based on the context outlined in the business problem. The complete code and model comparisons are available in the repository.
