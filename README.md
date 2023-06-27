# Predicting Email Classification as Spam Using Naive Bayes with CountVectorizer
This repository contains code for classifying emails as spam or ham (not spam) using the Naive Bayes algorithm. The code utilizes the Python programming language along with popular libraries such as pandas, numpy, seaborn, and scikit-learn.


## Introduction
Email spam detection is an important task in the field of data analysis and machine learning. The goal of this project is to predict whether an email is spam or ham based on its subject text. The code utilizes the Naive Bayes algorithm for classification, which assumes independence among predictors.


## Data
The dataset used for this project is stored in the `emails.csv` file. It contains various subjects of emails along with their classifications as either spam or ham. The dataset is loaded using the pandas library into a DataFrame called `spam_df`.

## Methods
1. Visualizing the Data: The script starts by providing an overview of the dataset, including the first 10 and last 10 rows, summary statistics, and information about the DataFrame.

2. Data Preprocessing: The script separates the dataset into two subsets: spam and ham. It calculates the percentages of spam and ham emails in the dataset. The text data of the emails is then transformed into a numerical representation using the CountVectorizer class from scikit-learn.

3. Model Training: The script splits the dataset into training and testing sets using the train_test_split function from scikit-learn. It then creates an instance of the MultinomialNB classifier and trains it on the training set.

4. Model Evaluation: The script evaluates the trained model by predicting the classes for both the training and testing sets. It calculates and visualizes the confusion matrix using seaborn's heatmap function. Finally, it prints the classification report, which includes metrics such as precision, recall, and F1-score.

## Results
The classification report provides insights into the performance of the Naive Bayes classifier for email spam detection. It includes metrics for both the training and testing sets, such as precision, recall, and F1-score.

