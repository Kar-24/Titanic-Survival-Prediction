# Titanic-Survival-Prediction
This project is a machine learning solution to the classic Titanic dataset from Kaggle’s Titanic competition using RandomForestClassifier

The goal is to predict whether a passenger survived the Titanic disaster based on features like age, gender, ticket class, and embarkation point.

Project Overview:
Dataset: Titanic train & test datasets (train.csv, test.csv)
Problem Type: Binary Classification (Survived = 0 or 1)
Algorithm Used: Random Forest Classifier (from scikit-learn)
Output: CSV submission file (submission.csv) with predictions

Steps to predict:

Data Preprocessing
Handle missing values:
Fill Age with median
Fill Embarked with mode
Fill Fare with median (test set)
Drop unnecessary columns: Cabin, Name, Ticket
Encode categorical variables:
Sex: male → 0, female → 1
Embarked: S → 0, C → 1, Q → 2
Model Training & Validation
Split training data (80% train, 20% validation)
Train a Random Forest Classifier
Evaluate with accuracy score
Prediction on Test Data
Use the trained model to predict survival on test.csv

Generate submission.csv with:
PassengerId
Pclass
Survived (predictions)

Validation Accuracy: ~82% (Random Forest, default parameters)
