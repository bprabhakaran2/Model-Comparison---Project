**Project Overview: **

In this practical application, the goal is to compare the performance of the classifiers, namely K Nearest Neighbor, Logistic Regression, Decision Trees, 
Support Vector Machines(SVM) and Random Forest on a Portugese Banking Institution dataset from UCI Machine Learning 
https://archive.ics.uci.edu/dataset/222/bank+marketing
The data is from a Portugese banking institution and is a collection of the results of multiple marketing campaigns.The dataset collected is related to 17 campaigns 
that occurred between May 2008 and November 2010, corresponding to a total of 79354 contacts 

The objective of this analysis is to predict whether a client will subscribe to a term deposit (y) based on their demographic, financial, campaign,contact, social and 
economic attributes.

By building a predictive model, the bank can focus its marketing efforts on clients who are most likely to respond positively. This will help improve the efficiency of 
telemarketing campaigns, save resources, and increase the overall success rate of term deposit subscriptions. The task also aims to identify the key factors that influence a client’s decision to subscribe.

**Summary of Findings:**
**Baseline Accuracy**
 Before Balancing : 80% of subscribers did not subscribe to a term deposit (target variable)
 After Balancing : 50% of subscribers did not subscribe to a term deposit (target variable)
 
**Best Performing Model:** 
For better generalization,Logistic Regression and SVM appear to be the most balanced models with moderate overfitting. These models have reasonable test performance and can be good choices for generalizing well to unseen data.
For better model interpretability,Logistic Regression is often favored because it is interpretable and easier to understand compared to models like SVM and Random Forest.
For higher accuracy, with overfitting,Random Forest and Decision Tree are highly accurate on the training data but fail to generalize well on the test data.
For high recall (i.e., detecting positive cases), SVM and Logistic Regression have good recall on the test data.

**Notebook Highlights**
Exploratory Data Analysis was performed to categorize and encode categorical and numerical data.
Dataset was split into Train and Test data for model prediction , propotional distribution between full , train and test data were compared

Baseline accuracy prediction of 80% indicated that 80% of customers have not subscribed for term deposit when data set was not balanced
Balancing the dataset using SMOTE indicated 50% of baseline accuracy

Model comparison : Performance of the Logistic Regression model to KNN algorithm, Decision Tree, SVM models and Random Forest models were performed.
Hyperparameter tuning and cross-validation was performed to optimize and generalize models.
Hyperparameters  were used for all classifiers to evaluate training time and accuracy on training and test datasets.

Plots: correlation heatmap of numeric columns, histogram and box plots for numerical and categorical column distribution, Target variable distribution , Model comparison

**Conclusion:**
Random Forest classifier and KNN has the highest training accuracy but shows some drop-off in test performance, possibly indicating overfitting.

Random Forest and SVM has highest test accuracy but a longer fit time, making it less practical for large datasets.

Decision Tree has high accuracy and very fast training time, but may suffer from overfitting due to the difference in train and test accuracy.

Overall Logistic Regression is relatively fast with decent performance in both train and test sets and is more suited for faster, less complex problems.
