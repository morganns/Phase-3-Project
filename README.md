# **Terry Stops Analysis: A Data-Driven Approach to Predicting Arrests**

## **Project Overview**

This project analyzes Terry Stops, a law enforcement practice where officers stop individuals based on reasonable suspicion.
The goal is to develop a predictive model that determines the likelihood of an arrest occurring during a Terry Stop, ensuring fairness, transparency, and accountability in policing.

## **Business & Data Understanding**

**Problem Statement**

Law enforcement agencies need data-driven insights to ensure fair and unbiased arrests.

This project aims to predict whether an arrest will occur during a Terry Stop using machine learning.

**Stakeholders**

Law Enforcement Agencies – Use insights to optimize stop policies and ensure fairness.
Policymakers & Civil Rights Organizations – Evaluate potential biases and recommend policy adjustments.
Citizens & Community Groups – Promote transparency and trust in law enforcement.

**Dataset Overview**

The dataset contains Terry Stops records, including demographics, stop resolutions, and officer characteristics.

It consists of 62,717 rows and 23 columns.

**Key Features**

Categorical Variables: Stop Resolution, Weapon Type, Precinct.

Numerical Variables: Officer YOB, Reported Hour, Day of Week.

**Data Preprocessing Steps**

✅ Handled missing values using median imputation.

✅ Categorical features encoded using Label Encoding.

✅ Feature Scaling applied with StandardScaler.

✅ Created additional features: Officer Experience, Peak Crime Hours, Weekend Stops.

✅ Addressed class imbalance using SMOTE.

## **Model Development**

Chosen Model: Logistic Regression

Why Logistic Regression?

Simple, interpretable, and effective for classification tasks.

Computationally efficient, making it ideal for large datasets.

Provides insights into key predictive features.

**Model Training Steps**

✅ Pipeline for Preprocessing & Training – Ensured structured workflow.

✅ Hyperparameter Tuning with GridSearchCV & Bayesian Optimization – Optimized C (Regularization), Solver, and Penalty.

✅ Decision Threshold Optimization – Adjusted to 0.42, reducing False Negatives.

✅ Final Model Selection – Best Logistic Regression model chosen based on F1-score and fairness assessment.

## **Model Evaluation**

**Key Performance Metrics**

✅ Classification Report: Precision, Recall, and F1-score analyzed.

✅ Confusion Matrix: Showed correct vs. incorrect predictions.

✅ ROC Curve & AUC Score: AUC improved from 0.84 to 0.89 after tuning.

✅ Precision-Recall Curve: Confirmed strong model performance in imbalanced data.

Observations from Further Model Tuning

✅ F1-score increased from 0.72 to 0.85.

✅ False Negatives reduced by 18%, improving Recall.

✅ Bias Testing revealed minor fairness variations across demographic groups.

✅ Decision Threshold Optimization helped achieve better Precision-Recall balance.

## **Findings & Recommendations**

**Findings**

✅ Predictive Features Identified – Stop Resolution, Weapon Type, and Reported Hour were the strongest predictors.

✅ Model Performance Improved – Fine-tuning and feature engineering enhanced the model's predictive power.

✅ Bias Testing Exposed Minor Variations – While generally fair, some demographic groups had slight accuracy differences.

**Recommendations**

1️⃣ Enhancing Law Enforcement Decision-Making

Use model insights to improve officer training on arrest justifications.

Deploy predictive analytics to support real-time law enforcement decisions.

2️⃣ Further Model Improvements

Explore ensemble learning models like Random Forest and Gradient Boosting for comparative analysis.

Implement deep learning techniques for further predictive power enhancements.

Continue monitoring model fairness to mitigate potential biases in arrest predictions.

3️⃣ Policy & Ethical Considerations

Collaborate with law enforcement agencies to ethically deploy predictive policing tools.

Conduct periodic fairness audits to ensure the model does not disproportionately impact specific communities.

Develop guidelines for the responsible use of AI in law enforcement.

## **Next Steps**

✅ Pilot the model in real-world policing scenarios to assess effectiveness in live decision-making.

✅ Continuously monitor and refine predictions based on feedback from law enforcement officers.

✅ Expand the dataset by incorporating additional variables such as officer training history, socioeconomic conditions, and location-based crime rates.

By implementing these recommendations, law enforcement agencies can enhance fairness, transparency, and accountability in policing, ensuring data-driven and just decision-making.