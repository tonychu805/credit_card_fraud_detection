### Introduction

We employ diverse predictive models to assess their precision in distinguishing between regular payments and fraudulent transactions. The dataset specifies that the features are scaled, and their names are withheld for privacy reasons. Despite this, we can examine key aspects of the dataset. Let's commence!

### Objectives

- Comprehend the limited distribution of the "small" dataset at our disposal. 
- Generate a sub-dataframe with a 50/50 ratio of "Fraud" and "Non-Fraud" transactions using the NearMiss Algorithm. 
- Identify the classifiers to be employed and evaluate their respective accuracies, selecting the one with the highest performance. 

### Summary:

- The transaction amounts are relatively modest, with an approximate mean of USD 88 across all transactions.
- No "Null" values are present, eliminating the need to devise methods for value replacement.
- The majority of transactions (99.83%) are classified as Non-Fraudulent, with Fraudulent transactions occurring only 0.17% of the time in the dataframe.

### Feature Technicalities:

- PCA Transformation: The data description indicates that all features underwent PCA transformation, a dimensionality reduction technique, except for time and amount.
- Scaling: It's important to note that for implementing PCA transformation, features must be scaled beforehand. In this instance, we assume that the dataset developers have scaled all the V features, although this is not explicitly stated.

### Results

- Accuracy on Logistic Regression Training data :  96.2%
- Accuracy on SVC Training data :  96.6%
- Accuracy on Decision Tree Training data :  93.6%