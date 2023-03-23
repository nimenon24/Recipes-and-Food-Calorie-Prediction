# Recipes-and-Food-Calorie-Prediction
A DSC80 Project

## Framing the Problem

Our prediction problem is: Predict the number of calories

The type of this problem is regression.

For our data cleaning, the process is detailed on [this website](https://nimenon24.github.io/Recipe-and-Ratings-from-Food.com-EDA/). 

Our response variable is the number of calories a recipe has. We chose calories because we have already started to explore it earlier in our EDA, and in addition to our familiarity with it, we thought it would be interesting to see what other ingredients or nutrients in food can influence calories. 

We chose to use R^2 as our metric, since we are using a regression model. R^2 is the proportion of the variance in the response variable that is explained by the predictor variables, and since that is between 0 and 1, we thought it was easier to understand. In addition, it is not dependent on sample size. 

At the current time, we know the features that were given to us in the data frames that we had merged together from Food.com. Some of these features include nutrients,minutes, and number of steps. We can use some of these features in our prediction as the date for all these recipes have come before 2022. 

## Baseline Model


We decided to use a linear regression model as our baseline model. The features we chose were `carbohydrates`, `protein`, and `n_ingredients`. 

When we plotted `protein` and `calories`, as well as `carbohydrates` and `calories`, we saw that the relationship seemed to appear linear. 

<iframe src="assets/protein_cal.html" width=800 height=600 frameBorder=0></iframe>

<iframe src="assets/carbs_cal.html" width=800 height=600 frameBorder=0></iframe>

In our baseline model, we have 2 continuous quantitative variables: `protein` and `carbohydrates`. We also have 1 discrete quantitative variable, `n_ingredients`. 

The performance of our model was R^2 which was accuracy was about 0.8025781014688295
. Based on the accuracy score, this suggests that our model is pretty “good” in predicting a linear relationship. We decided this because our score for R^2 is fairly close to 1 which is where the r^2 score tells us that it is a good linear fit. 









