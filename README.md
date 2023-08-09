# DSC540AdvancedMachineLearning
Depaul Advanced Machine Learning class taken from Jan 3 2022 to March 20 2022.

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
