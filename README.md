# Phishing-Website-Detection

Introduction:

The goal of this project is to build a machine learning model that can predict whether a given website is a phishing website or not. Phishing websites are designed to look like legitimate websites to trick users into entering their sensitive information, such as passwords and credit card numbers. Detecting and blocking phishing websites is crucial for protecting users' online security and privacy.

Data:

The dataset used in this project is called 'phishing.csv'. The datset used in this project is a collection of website URLs for 11000+ websites. Each sample has 30 website parameters and a class label identifying it as a phishing website or not (1 or -1).


Preprocessing & Exploratory Data Analysis:

We started by importing the necessary libraries, including Pandas for data manipulation, NumPy for numerical computations, Matplotlib and Seaborn for data visualization, and Scikit-learn for machine learning algorithms. We also suppressed the warnings to avoid any clutter in the output. Next, we read the dataset into a Pandas DataFrame and dropped the 'Index' column as it was not necessary for our analysis. We then checked for missing values and unique values in the dataset and printed a summary of the dataset using the info() and describe() methods. We found that there were no missing values in the dataset, and all the features were numerical. We also plotted a histogram for each feature to visualize the distribution of values. We then created a correlation matrix heatmap to identify the correlations between features, which could help us in feature selection.


Model Selection:

After exploring the dataset, we split the data into training and testing sets using the train_test_split() method from Scikit-learn. We then trained a Logistic Regression model on the training set and evaluated its performance on the testing set. We also calculated the confusion matrix and classification report for the model. Next, we used a Decision Tree Classifier and performed a randomized search to find the best hyperparameters for the model. We then trained the model with the best hyperparameters and evaluated its performance on the testing set. We also calculated the confusion matrix and classification report for the model. Next, we used a Random Forest Classifier and performed a grid search to find the best hyperparameters for the model. We then trained the model with the best hyperparameters and evaluated its performance on the testing set. We also calculated the confusion matrix and classification report for the model. Finally, we used a SVM Classifier and performed a grid search to find the best hyperparameters for the model. We then trained the model with the best hyperparameters and evaluated its performance on the testing set. We also calculated the confusion matrix and classification report for the model.

Our results showed that the Decision Tree Classifier performed the best among all the models, with an accuracy of 97.1% and an F1 score of 0.970 for the positive class. The Logistic Regression, Random Forest Classifier and SVC also performed well with accuracies of 93.6%, 96.4% and 97 respectively.


Conclusion:

In conclusion, our project demonstrates the effectiveness of machine learning algorithms in identifying phishing websites. The Decision Tree Classifier, in particular, showed excellent performance and can be used to build an efficient phishing detection system.

