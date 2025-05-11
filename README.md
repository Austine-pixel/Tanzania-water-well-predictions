# Predicting Water Pump Failures in Tanzania 
## Objective
 Predict whether a water pump is:
 
•	Functional

•	Needs repair

•	Non-functional
The goal is to support efficient maintenance and resource allocation in rural Tanzania.
________________________________________
## Data Source
•	Competition: DrivenData - Pump It Up Challenge

•	Features include: location data, construction year, installer, water quality, extraction type, etc.

•	Target variable: status group (categorical)
________________________________________
## Technologies Used
•	Python

•	pandas, NumPy, seaborn

•	scikit-learn for modeling and evaluation

•	imbalanced-learn for handling class imbalance (SMOTE)
________________________________________
## Preprocessing Steps
•	Handled missing values and dropped uninformative columns.

•	Combined low-frequency categorical variables.

•	Encoded categorical features using One-Hot Encoding.

•	Balanced classes using SMOTE.
________________________________________
## Models Tried
•	Logistic Regression

•	Random Forest Classifier - Best performer

•	Hyperparameter tuning using GridSearchCV.
________________________________________
## Evaluation Metrics
Final Model (Random Forest Classifier after SMOTE and tuning):

Metric&nbsp;&nbsp;Score

Accuracy&nbsp;&nbsp;80.89%

F1-Score&nbsp;&nbsp;0.80

Precision/Recall (Class 1 - needs repair)	Improved, but still limited
________________________________________
## Key Findings
•	Random Forest outperforms Logistic Regression in both accuracy and class balance.

•	SMOTE helps improve recall for underrepresented classes.

•	Construction year and location are strong predictors of pump condition.
________________________________________
## Recommendations
•	Deploy the tuned Random Forest model as a baseline for real-world use.

•	Focus future improvements on better detecting the "Needs Repair" class.

•	Collect more balanced and recent data to improve class generalization.
