Student Performance Factors Analysis
Project Overview

This project analyzes and predicts student academic performance using the Student Performance Factors dataset from Kaggle. The dataset contains 10,000 records and 20 features representing academic, personal, and socio-environmental factors that influence exam outcomes.

The goal of this project is to:

Perform Exploratory Data Analysis (EDA) to identify key patterns and correlations.

Visualize relationships between variables such as Hours_Studied, Attendance, Parental_Involvement, and Exam_Score.

Build a Multi-Layer Perceptron (MLP) deep learning model to classify students as high or low performers.

Provide insights to help educators and policymakers enhance student learning strategies.

Dataset

Source: Kaggle – Student Performance Factors Dataset

Number of Records: 10,000
Number of Features: 20 (including target variable Exam_Score)

Key Features Include:

Hours_Studied

Attendance

Parental_Involvement

Motivation_Level

Teacher_Quality

School_Type

Internet_Access

Previous_Scores

Extracurricular_Activities

Exam_Score (Target)

Methodology

Data Preprocessing:

Handled missing values (mean for numeric, mode for categorical)

Encoded categorical variables using One-Hot Encoding

Standardized numeric features using StandardScaler

Created a binary target variable Performance_Level (Exam_Score >= 60)

Exploratory Data Analysis (EDA):

Histograms, boxplots, and scatterplots for numeric features

Correlation heatmap for relationships between numeric features

Countplots for categorical variables

Model Development:

Multi-Layer Perceptron (MLP) with two hidden layers (128 and 64 neurons) and Dropout

Sigmoid output for binary classification

Adam optimizer and binary crossentropy loss

EarlyStopping on validation loss

Model Evaluation:

Accuracy, precision, recall, F1-score

Confusion matrix and ROC-AUC

Visualization of training/validation loss and accuracy

Insights

High-performing students generally have higher study hours, attendance, and motivation levels.

Parental involvement and teacher quality positively affect academic outcomes.

Students in private schools or with internet access perform better.

Top predictors of exam success: Hours_Studied, Previous_Scores, Motivation_Level, Teacher_Quality.

Future Scope

Extend the model for regression to predict exact exam scores.

Incorporate additional features like mental health, diet, and classroom engagement.

Explore ensemble models or advanced neural networks for improved accuracy.

Deploy a real-time monitoring system for early identification of at-risk students.