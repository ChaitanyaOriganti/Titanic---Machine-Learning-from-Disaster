This repository contains a machine learning project aimed at predicting the survival of passengers aboard the Titanic using various classifiers. Below is an overview of the project structure, dataset information, and the classifiers used.

Project Overview
The goal of this project is to predict whether a passenger survived the sinking of the Titanic based on features such as gender, ticket class, age, and more. The dataset is split into a training set (train.csv) and a test set (test.csv). The provided gender_submission.csv file offers an example of the expected format for submission.

Data Dictionary
Here is a breakdown of the variables in the dataset:

Survival: 0 = No, 1 = Yes (This is the target variable)
Pclass: Ticket class - 1 = 1st (Upper), 2 = 2nd (Middle), 3 = 3rd (Lower)
Sex: Gender of the passenger
Age: Age in years (fractional if less than 1, xx.5 if estimated)
SibSp: # of siblings / spouses aboard the Titanic
Parch: # of parents / children aboard the Titanic
Ticket: Ticket number
Fare: Passenger fare
Cabin: Cabin number
Embarked: Port of Embarkation - C = Cherbourg, Q = Queenstown, S = Southampton
Variable Notes
Pclass: A proxy for socio-economic status (SES)
Age: Age is fractional if less than 1; if estimated, it is in the form of xx.5
SibSp: Defines family relations - Sibling = brother, sister, stepbrother, stepsister; Spouse = husband, wife
Parch: Defines family relations - Parent = mother, father; Child = daughter, son, stepdaughter, stepson
Some children traveled only with a nanny, hence Parch=0 for them.
Machine Learning Classifiers
The following classifiers were used to predict survival:

KNeighborsClassifier
RandomForestClassifier
Neural Network
XGBClassifier
SVC (Support Vector Classifier)
LightGBM
