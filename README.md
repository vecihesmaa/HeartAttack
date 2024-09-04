# Heart Disease Prediction

This project aims to predict the presence of heart disease in patients using a logistic regression model. The dataset used for this project is `heart.csv`, which contains various features related to the patient's health.

# Table of Contents
- Project Overview.
- Installation.
- Dataset
- Exploratory Data Analysis (EDA)
- Data Preprocessing
- Modeling
- Evaluation
- Conclusion

# Project Overview
The goal of this project is to use machine learning techniques to predict whether a patient has heart disease based on several medical attributes. Logistic regression is used as the primary model for classification.

# Installation
To run this project, you need to have the following libraries installed:
bash
```pip install numpy pandas matplotlib seaborn scikit-learn ```

# Dataset
The dataset heart.csv contains the following features

- [Download here](https://www.kaggle.com/datasets/rashikrahmanpritom/heart-attack-analysis-prediction-dataset)

age: Age of the patient
sex: Gender of the patient (1 = male; 0 = female)
cp: Chest pain type (4 values)
trtbps: Resting blood pressure (in mm Hg)
chol: Serum cholesterol in mg/dl
fbs: Fasting blood sugar > 120 mg/dl (1 = true; 0 = false)
restecg: Resting electrocardiographic results (values 0, 1, 2)
thalachh: Maximum heart rate achieved
exng: Exercise-induced angina (1 = yes; 0 = no)
oldpeak: ST depression induced by exercise relative to rest
slp: The slope of the peak exercise ST segment
caa: Number of major vessels (0-3) colored by fluoroscopy
thall: Thalassemia (3 = normal; 6 = fixed defect; 7 = reversible defect)
output: Diagnosis of heart disease (1 = disease; 0 = no disease)

# Exploratory Data Analysis (EDA)
EDA was performed using Seaborn and Matplotlib. Some key visualizations include:

Count plots for categorical variables.
Pair plots for numerical variables to examine relationships.

# Data Preprocessing
Categorical variables were converted to dummy variables.
Numerical features were scaled using StandardScaler.

# Modeling
The logistic regression model was trained on the preprocessed data:
logreg = LogisticRegression()
logreg.fit(xtrain, ytrain)

# Evaluation
The model was evaluated on the test set, achieving an accuracy of approximately 84.78%.
print("Test Accuracy:", accuracy_score(ypred, ytest))

# Conclusion
The logistic regression model provides a good baseline for predicting heart disease. Further improvements can be made by tuning hyperparameters or exploring more complex models.

You can modify the content according to any specific details or additional features you want to highlight.
