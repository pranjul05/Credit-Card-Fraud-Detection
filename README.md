# -Credit-Card-Fraud-Detection
Credit card fraud poses a major challenge for both financial institutions and their customers. The key difficulty for financial institutions lies in detecting fraudulent transactions in real-time while minimizing false positives.

The objective of this project is to build a machine learning model capable of accurately identifying fraudulent credit card transactions while reducing false positive rates. The model is trained on historical data to detect patterns and anomalies that indicate fraudulent behavior. The dataset used for this project was sourced from Kaggle and can be accessed through the following link. https://www.google.com/url?q=https%3A%2F%2Fwww.kaggle.com%2Fmlg-ulb%2Fcreditcardfraud%3Fselect%3Dcreditcard.csv"

The dataset consists of credit card transactions made by European cardholders in September 2013, spanning a two-day period. Out of 284,807 total transactions, 492 were identified as fraudulent, resulting in a highly imbalanced dataset, where the positive class (fraudulent transactions) constitutes just 0.172% of the data.

All input variables in the dataset are numerical and have undergone PCA (Principal Component Analysis) transformation to ensure confidentiality, with the original features and additional background details unavailable. The target variable, 'Class,' is labeled as 1 for fraud and 0 for non-fraudulent transactions.

We began with an in-depth exploratory data analysis (EDA), performing both univariate and bivariate analysis for all features. Given the significant class imbalance, we applied under-sampling techniques to balance the dataset.

To evaluate the relationships between features, we used a correlation heatmap. Additionally, outliers were identified and removed using boxplots.

Due to the high dimensionality of the dataset, visualizing patterns beyond three dimensions is challenging. To overcome this, we applied dimensionality reduction techniques to visualize the data effectively.

Since this is a classification problem, we implemented several classification models and evaluated them using cross-validation scores to determine the best fit for our data. Some of the models that we have used are:

-LogisticRegression

-KNeighborsClassifier

-Support Vector Classifier

-DecisionTreeClassifier

We have used sklearn cross_val_score to compare model performances, for this we have checked which model has best mean average accuracy over given number of folds. We tried to look for the best set of paramters for models using gridsearch.

We have used these to evaluate our model:

-Cross_val_score

-ROC AUC Score

-ROC Curve

-Confusion Matrix, Classification report

-Average precison score, Area under precision recall curve

And we found out that SVC and Logistic regression have best cross validation score. Also, we observed that SVC has better ROC AUC Score.


