## NFL Group

Features: FG_A, FG_Per, SP_A XP_Per

Stadiums, Games, Plays
No slide number
Bad chart labels (FG_A, FG_per?)
Binning for latitude
Do they take altitude as a feature?

COnsidered imbalanced data - under / oversampling
Model level - cost sensitive learning? -
Feature selection
Model running - is accuracy on validation set? What's the size?

GridSearch for hyperopt!
25k entries for validation

Suggestions:
More metrics other than accuracy can give you a better idea whether it's better to have imbalanced data at 80% accuracy or balanced at 85%

---

## Shooters Gotta Shoot

Predicting 3-point shots made by any player in NBA

> Col, Sam, Phil, ?, ?

+ 3-point attempts, rate, shooting percentage
+ Related works - best game strategy based on plays that end with 3-point shots.
+ Light Gradient Boosting Machine - LGBM?

+ 10 years of data
+ Using cross validation - 10-fold
+ "Run models for each subset of features for each model" sounds like brute-forcing, maybe it's worth to do the feature engineering beforehand using PCA, SVD, or at least some correlation analysis?
+ They may apply PCA or SVD for dimensionality reduction

---

## Secretariat - predicting horse races

Types of bet:

+ Outright win
+ Place - any of top 3
+ Quinella - any of top 2
+ Quinella Place - both top 2

More on prediction:

+ Predictions of 4 horses
+ Predict features to be bet consistently in order to make money
+ Probabilities of top 2 or top 3
+ Regression model to compute probability instead of binary classification

Data

+ Using Kaggle
+ Each horse has an attribute
+ **Kelly criterion** - automatically optimizes the bet based on perceived advantage on the bet <<

---

Predicting congressional election outcomes using congression

> Bryan, Connor, Patrick, Luke

Data

+ Demographic (population, density, blue-collar workers, unemployed, ethnicity, district size, within 100 of DC?)
+ Missing data was ignored
+ Equal number of samples in each class (dem 56.5%, 42.8%)

Results and next steps

+ Preliminary results for CART
+ Regression instead of binary classification
+ Not using past results as features
+ Voter turnout to be used as feature (voters / pop)
