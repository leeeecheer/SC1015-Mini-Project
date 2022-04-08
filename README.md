# SC1015-Mini-Project

# About
This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses on predicing loans based on customer behaviour. For a detailed walkthrough, please view the source code in this order:

1. Data Extraction
2. Data Visualization
3. Data Resampling and Splitting
4. Decision Tree and Random Forest
5. Logistic Regression

# Contributors
@sunwen_12
@CH-2902
@leeeecheer 

# Problem Definition
Given the profile of an individual, how can we use these variables to predict the probability of him/her defaulting on a loan that is about to be taken?
Which model best predicts the best outcome?

# Notebooks
## Data Cleaning and Preparation
The code in this notebook is cleaned to ensure that there are no null values or values which do not fit the category of the column. For data cleaning, we removed the ID column as we find it unnecessary since we can use the indexes of the column. For data preparation, we changed the Risk_Flag column and converted it to a Risk_Class column as the former is a categorical variable with integer values which we converted to No Risk and Risk which are object values.

## Exploratory Data Analysis
The code in this notebook is to extract the individual variables from the dataset for visualisation. We have conducted both Uni-variate and Bi-variate analysis to aid us in our visualisation. For Uni-variate visualisation, we checked each variable through the use of barplots and by printing the values of those with too many values(CITY). For Bi-variate visualisation, we used boxplots and kdeplots to compare the numerical variables to the Risk_Class column. When comparing categorical variables to Risk_Class, we used barplots and heatmaps. For complex relationships where we analysed the numeric variables based on the Risk_Class, we used a jointplot and a correlogram to visualise the data.

## Machine Learning(Mulitvariate Classfication Tree and Random Forest)
The code in this notebook is for us to find the best model in predicting how likely a person will default a loan. For this notebook, it is split into 4 parts. Before we started, we used one hot encoder to convert categorical variables into numbers. For our first model, we did Mulitvariate Classification for numeric, categorical, numeric and categorical variables to predict the Risk_Class. For our second model, we upsampled the data for Risk_Class as there is a huge imbalance. For the third model, we made use of Random Forest to ensemble mulitple trees for a better prediction. Finally, we looked for the model that produces the best accuracy for our tree with respect to its depth.

## Machine Learning(Logistic Regression)

Conclusion
Popularity and budget have low linear correlation value with ratings (watch out for bandwagons 🤣)
Popularity of the casts and crews have higher linear correlation value with ratings
Resampling imbalanced data improved model performance especially on the minority class
Logistic Regression did not perform well with non-linearly correlated variables
Neural Networks along with SMOTEENN resampling method consistently did well in predicting good movies after 100 training attempts (around 72% accuracy, 70% recall)
Yes, it is possible to predict if a movie is good with acceptable amount of accuracy and recall
What did we learn from this project?
Handling imbalanced datasets using resampling methods and imblearn package
Neural Networks, Keras and Tensorflow
Logistic Regression from sklearn
API Usage
Other packages such as tqdm, json, requests
Collaborating using GitHub
Concepts about Precision, Recall, and F1 Score
