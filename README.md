# DSC540AdvancedMachineLearning
Depaul Advanced Machine Learning class taken from Jan 3 2022 to March 20 2022.

Home Work Project 1: 
I used the Breast Cancer Wisconsin dataset from the uci archive website to load it into pandas where I had to investigate the column types, check the statistical summary of numerical features with a goal determining the variables with the largest and smallest values. I derived a correlation heatmap, which helped to determine any largely correlated variables. I went a head to use sklearn's tran_test_split() function to create the split of the dataset.
I initiated the Gaussian Naive Bayes and logistic regression classifiers:
- to fit the model
- make predictions
- calculated the training and testing accuracies of the model
Finally, derived the models' performances using:
- Recall(Sensitivity)
- Specificity
- Precision
- False Positive Rate
- F1 Score

Also, created a for loop where i fitted the KNN model using various values of K, made predictions and calculated the accuracy scores for training and testing datasets. Created a validation curve based on each K value and the corresponding train and test accuracies.

In the last part of this home work project, I implemented feature engineering where I scaled the features by standardizing train and test sets.

Home Work Project 2:
I explored the publicly available data from LendingClub.com.

The group project sought to classify customers into those who would or would not accept the marketing campaign. Identifying customers who are more likely to accept the campaign will assist companies in using their marketing resources more effectively. The original dataset included 2,240 observations and 29 columns.

We conducted data exploration, data visualization, and preprocessing to clean the data, including examining and addressing missing values and outliers.

We used three versions of the dataset in our analysis, including:

1. A standardized dataset.
2. A standardized dataset that used Synthetic Minority Oversampling Technique (SMOTE) and Random Undersampling to address class imbalance.
3. A standardized principal component analysis dataset using the top 15 components that accounted for 90% of the variance.


For each of the datasets, we used the following classifiers and compared their base model performance to their performance using the best parameters identified using GridSearchCV.

- Logistic Regression
- Support Vector Machines
- KNN
- Decision Tree
- Random Forest
- Adaboost
- Gradient Boosting
We used the following evaluation metrics:

- Training accuracy
- Validation accuracy
- Recall
- Specificity
- Precision
- Balanced Accuracy
- F1 score
- Difference between training and validation accuracy
- Profit

The dataset indicated that each contact cost the company $3, and each campaign acceptance produced a revenue of $11. Using this data, we calculated the following profit evaluation metric:

Profit = (True positives x $11 revenue) - (False positives x $3 cost) - (False negatives x $11 lost revenue)

We balanced these metrics to determine our two best models. We then evaluated the two best models on the set aside test dataset. Our results indicated the RandomForest Classifier produced the best overall metrics, including the highest profit score.
