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

This dataset is from LendingClub before it went public.

The lending data from 2007 to 2010 was used to classify and predict whether or not the borrower paid back their loan in full.

Home Work Project 3:
I analyzed CO and NOX gas emissions from a power plant. 

I predicted CO using all other variables through:
- linear regression.
- Support Vector Regression
- Random Forest Regression 

Measured the model's performed using R-Squared and RMSE.

Used GridSearchCV to tune the different hyper-parameters.

Applied PCA to transform the data.

Used the PCA transformed data to perform regression with hyper parameters tuning using the models:
- Linear Regression
- Random Forest Regression
- RBF Kernel Support Vector Regression

Lastly, we converted CO target values into binary form by comparing them to a threshold. 0 - 3mg/m^3 was the range of max 8 hour avg used. This was done to facilitate classification. 

Home Work Project 4:
This home work was about using Bayesian analysis to estimate the market share for a new drug. 

We also analyzed medical diagnosis using Bayes Nets. 




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
