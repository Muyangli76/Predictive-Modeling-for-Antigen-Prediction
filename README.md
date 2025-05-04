# Predictive-Modeling-for-Antigen-Prediction
(Details are excluded for confidentiality) Helping Sanofi optimize the use of Raman spectroscopy data to enhance antigen production
Overview
This project applies an EKF to improve the accuracy of model predictions, specifically in time-series prediction corrections based on initial errors. It includes several trial methods to assess different strategies for improving predictions.

## Features:
- EKF State Estimation: Implements an EKF to update state estimates.
- Prediction Correction: Corrects model predictions by comparing them with measured values and adjusting using Kalman Gain.
- Multiple Trial Implementations: Evaluates various methods (e.g., MAE, Kalman Gain averaging) for correction over time.
- Data Handling: Efficiently handles large datasets and makes corrections step by step over the time series.

## Key Challenges

- **Model Integration**: Integrating the Random Forest Regressor with the EKF model to allow real-time prediction corrections is complex, requiring a deep understanding of both machine learning and filtering algorithms.

- **Cross-Model Data Alignment**: Synchronizing and ensuring consistency between datasets (e.g., BatchID/SAP, Age values) for accurate corrections adds significant complexity.

- **Data Handling**: Managing and preprocessing large datasets (440,067 rows) while ensuring data quality (no missing values, outliers) is essential for model success.

- **Feature Engineering**: Properly extracting, scaling, and transforming features to ensure accurate model predictions requires careful attention to relationships between variables.

- **Model Evaluation**: Evaluating model performance across different subsets and ensuring generalization while avoiding overfitting/underfitting requires careful validation strategies.


## Result Discussion

![image](https://github.com/user-attachments/assets/acd11a59-5a71-4002-960f-7c806b554ed6)


![image](https://github.com/user-attachments/assets/42e978d0-1204-4959-ba06-de34d22584ef)


![image](https://github.com/user-attachments/assets/5a4cc005-bf6d-47ff-9234-46a48c9e1318)
