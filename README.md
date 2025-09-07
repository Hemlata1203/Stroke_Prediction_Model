# 🧠 Stroke Prediction System

A machine learning-based stroke prediction system that leverages demographic, lifestyle, and medical history data to predict the likelihood of an individual experiencing a stroke. The project applies multiple ML algorithms, interpretable AI techniques, and evaluation metrics to provide meaningful insights for healthcare decision-making.

## 📌 Project Overview

Stroke is one of the leading causes of death and disability worldwide. Early prediction of stroke risk can help in timely intervention and prevention. This project develops a stroke prediction system using machine learning models to analyze healthcare data and identify individuals at high risk.

## 🎯 Objectives

Early Identification: Detect high-risk individuals for timely intervention.

Personalized Risk Assessment: Provide patient-specific stroke risk analysis.

Clinical Decision Support: Assist healthcare professionals in recommending lifestyle modifications and treatments.

## 🗂 Dataset

Source: [Kaggle](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset)

Features: medical history, BMI, Demographics,  lifestyle, and clinical indicators.

Challenge: Highly imbalanced dataset (≈ 5% stroke cases).

Balancing Technique: SMOTE (Synthetic Minority Oversampling Technique) was used to handle class imbalance.

## 🔧 Data Preprocessing

Data Cleaning: Missing BMI values predicted using Decision Tree.

Feature Encoding: Handled categorical variables.

Data Balancing: Applied SMOTE to balance the dataset.

Exploratory Data Analysis (EDA): Visualized correlations between age, BMI, lifestyle, and stroke risk.

# 🤖 Machine Learning Models Used

The following ML models were implemented and compared:

Random Forest Classifier

Accuracy: ~94% (Tuned)

Recall (Stroke Patients): Very low (~2%)

Logistic Regression

Accuracy: ~76%

Best recall and F1-score among all models

Final selected model due to better balance between recall and precision

Support Vector Machine (SVM)

Accuracy: ~76%

Recall and F1-score lower than Logistic Regression

## 📊 Model Evaluation

Metrics Used: Accuracy, Precision, Recall, F1-score, ROC-AUC

Key Insight:

While Random Forest had higher accuracy, Logistic Regression outperformed others in recall and F1-score, which is crucial for stroke detection.

False negatives (missing a stroke case) are more critical than false positives in healthcare prediction.

## 🔍 Model Interpretability

To make the model explainable and transparent:

LIME (Local Interpretable Model-Agnostic Explanations): Explained feature contributions for individual predictions.

ELI5: Provided global feature importance and coefficients for Logistic Regression.

These tools helped interpret how features like Age, BMI, Hypertension, and Smoking Status influenced predictions.

## ✅ Conclusion

Age is a strong predictor of stroke risk.

Logistic Regression with tuning provided the best recall and F1-score, making it the final choice.

Explainability tools (LIME & ELI5) made the model transparent for business stakeholders and clinicians.

This system can serve as a decision-support tool in healthcare for early stroke prevention.

## 💼 Business Impact

This project demonstrates how machine learning can solve business problems in healthcare and insurance:

Hospitals & Clinics: Reduce emergency treatment costs by identifying high-risk patients early and providing preventive care.

Health Insurance Companies: Improve risk assessment models for policy pricing and claims prediction.

Pharmaceutical Companies: Target preventive drugs and therapies more effectively to populations at risk.

Government & NGOs: Allocate healthcare resources efficiently to reduce stroke-related disability and mortality rates.

Employers (Corporate Wellness Programs): Use predictive analytics to design wellness plans, reducing employee absenteeism and healthcare expenses.

By preventing strokes, businesses save on treatment costs, insurance payouts, and workforce productivity losses, making this model not just a healthcare innovation but also a business strategy enabler.

## 🚀 Use Cases

Healthcare Providers: Assist in identifying at-risk patients for preventive care.

Insurance Companies: Risk profiling for health policies.

Research & Analytics: Understanding correlations between lifestyle, health conditions, and stroke risk.


✨ This project demonstrates how machine learning can be used to address real-world healthcare challenges while also creating measurable business value.
