# Titanic-Survival-Training-Model
This repository consists of two training models with the same goal of predicting the number of survivors aboard the RMS Titanic given certain factors like Age, Sex etc. The following is a step-by-step description on how each model works.
## First Training Model 
1. Data is loaded.
2. Features are checked for missing values.
3. The feature with the least amount of missing values is selected.(In this case 'Sex' is chosen)
4. We proceed to construct a single feature logistic regression model.
## Second Training Model
1. Data is loaded.
2. EDA (Exploratory Data Analysis) is utilised to explore the size and shape of the data.
3. We calculate the percentage of missing values in each attribute.
4. A heatmap is used to better accentuate the missing values.
5. We then proceed to fill in the missing values by predicting them based on another given feature. We use a correlation matrix to find the most suitable feature for this(In this case Pclass has the highest correlation value).
6. The features that we don't need are dropped.
7. We split our training set in an 80|20 ratio,i.e. predicting the last 20% of the observations of our training dataset with a model produced from the first 80%. This is a local validation technique.
8. We then proceed to use logistic regression to make our predictions. We calculate our accuracy percentage using the confusion matrix formula.
