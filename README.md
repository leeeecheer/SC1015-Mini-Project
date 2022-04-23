# SC1015-Mini-Project

# About
This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses on predicing loans based on customer behaviour. For a detailed walkthrough, please view the source code in this order:

1. Data Preparation and Cleaning
2. Exploratory Data Analysis
3. Machine Learning
4. Logistic Regression
5. Further Insights

# Contributors
@sunwen_12
@CH-2902
@leeeecheer 

# Problem Definition
Given the profile of an individual, how can we use these variables to predict the probability of him/her defaulting on a loan that is about to be taken?
Which model best predicts the best outcome?

# Datasets
We have made several datasets so that each dataset will be ready for modeling or exploration when we want to further analyse it.

# Notebooks
## Data Cleaning and Preparation
The code in this notebook is cleaned to ensure that there are no null values or values which do not fit the category of the column. For data cleaning, we removed the ID column since we can just use the indexes of the column. For data preparation, we added the Risk_Class column which is the representative of the Risk_Flag column but with object values instead.

## Exploratory Data Analysis
The code in this notebook is to extract the individual variables from the dataset for visualisation. We have conducted both Uni-variate and Bi-variate analysis to aid us in our visualisation. For Uni-variate visualisation, we checked each variable through the use of barplots and by printing the values of those with too many values(CITY). For Bi-variate visualisation, we used boxplots and a pairplot to compare the numerical variables to the Risk_Class column. When comparing categorical variables to Risk_Class, we used barplots and heatmaps. For complex relationships where we analysed the numeric variables based on the Risk_Class, we used a jointplot and a correlogram to visualise the data.

## Machine Learning
The code in this notebook is for us to find the best model in predicting how likely a person will default a loan. For this notebook, it is split into 4 parts. Before we started, we used one hot encoder to convert categorical variables into numbers. For our first model, we did Mulitvariate Classification for numeric and categorical variables to predict the Risk_Class. For our second model, we upsampled the data for Risk_Class as there is a huge imbalance and did Multivariate Classification for numeric and categorical variables to see the change in accuracy. For the third model, we made use of Random Forest to ensemble mulitple trees for a better prediction. Finally, for our fourth model, we downsampled our data and used Random Forest to prevent data leakage from upsampling. We also found the most important features in predicting Risk_Class.

## Machine Learning(Logistic Regression)
The code in this notebook is for us to explore other methods that were not taught in the lectures. We have decided to use logistic regression as it is a model that allows us to predict categorical responses with our predictors. This is suitable for our dataset as we are trying to predict whether a person is going to default a loan(Risk or No Risk). For this model, we used one hot encoder and upsampled our data so that the response variable will not be imbalanced. This model has helped us learn how to apply models that we find online to help us in our predictions.

## Further Insights
The code in this notebook is to use what we learn from our EDA and Machine Learning to gain further insights. The information that we found will be useful for banks in India to seive out individuals with higher risk and take the necessary precautions.

# Learning Points
* Resampling datasets with imbalanced data
* Logistic Regression from sklearn
* Feature Importance
* Dealing with huge datasets
* Collaborating using GitHub

# References
* https://www.kaggle.com/datasets/subhamjain/loan-prediction-based-on-customer-behavior?datasetId=1532161&sortBy=voteCount
* https://slidesgo.com/
* https://scikit-learn.org/stable/
