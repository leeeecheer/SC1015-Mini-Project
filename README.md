# SC1015-Mini-Project

# About
This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses on predicing loans based on customer behaviour. For a detailed walkthrough, please view the source code in this order:

1. Data Extraction
2. Data Visualization
3. Data Resampling and Splitting
4. Decision Tree and Random Forest
5. Logistic Regression

# Contributors
@leeeecheer 
@sunwen_12
@CH-2902

# Problem Definition
Given the profile of an individual, how can we use these variables to predict the probability of him/her defaulting on a loan that is about to be taken?
Which model best predicts the best outcome?

# Notebooks
## Data Cleaning
Neural Networks

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
