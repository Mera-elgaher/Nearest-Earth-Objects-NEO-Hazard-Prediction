**Nearest Earth Objects (NEO) Hazard Prediction**
**Project Overview**
I worked on predicting whether a Nearest Earth Object (NEO) is hazardous using a dataset from NASA. This prediction is critical for planetary defense and identifying potential threats to Earth. I used machine learning models to achieve this goal, focusing on data preprocessing, handling imbalanced classes, and evaluating the model's performance.

Dataset : NASA Nearest Earth Objects 1910-2024
--------------------------------------------------
**Table of Contents**
Project Overview
Data Importing and Cleaning
Exploratory Data Analysis (EDA)
Data Preprocessing
Model Training and Evaluation
Findings and Insights
Conclusion
------------------------------------------------------------------
**1-Data Importing and Cleaning**
I started by importing the dataset and cleaning it. This included:

Handling Missing Values: Missing values in numerical columns were replaced with the mean, and missing categorical data was filled with the mode.
Removing Duplicates: Duplicates were identified and removed to ensure the dataset's integrity.
-------------------------------------------------
**2-Exploratory Data Analysis (EDA)**
To understand the data better, I performed EDA:
Visualizations: I used seaborn and matplotlib to create plots showing the distribution of hazardous versus non-hazardous objects.
Heatmap: I generated a correlation heatmap to visualize relationships between numerical features.
-------------------------------------------------------
3-**Data Preprocessing**
I prepared the data for modeling by:

Encoding Categorical Variables: I used one-hot encoding to convert categorical variables into numerical format.
Scaling Features: I normalized the features using StandardScaler.
Handling Imbalanced Classes: Since the target variable, is_hazardous, was imbalanced, I used SMOTE (Synthetic Minority Over-sampling Technique) to balance the class distribution.
------------------------------------
**4-Model Training and Evaluation**
I trained and evaluated two machine learning models:

Random Forest Classifier: I trained this model and evaluated it using precision, recall, F1-Score, and ROC-AUC score.
Gradient Boosting Classifier: I also trained a Gradient Boosting model to compare its performance against the Random Forest classifier.
------------------------------------------------
**Evaluation Metrics Used:**

Confusion Matrix
ROC-AUC Curve
Precision, Recall, F1-Score
----------------------------
**Findings and Insights**
Class Imbalance: Addressing the class imbalance using SMOTE significantly improved model performance.
Random Forest vs Gradient Boosting: Both models performed well, with the Gradient Boosting classifier providing slightly better precision and recall in certain scenarios.
Feature Importance: I identified key features that contributed the most to predicting hazardous objects, which will be useful for future research and model improvement.
----------------------------------
**Conclusion**
This project highlighted the importance of data preprocessing, especially when dealing with imbalanced datasets. The models provided valuable insights into predicting hazardous NEOs, which can be crucial for future planetary defense initiatives. Further steps could include hyperparameter tuning and exploring additional models like XGBoost.
