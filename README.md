# stroke-risk-classification
Machine Learning models to predict stroke risk using classification algorithms like Logistic Regression, Random Forest, SVM, and Stacking. Includes data preprocessing, model evaluation, and feature importance analysis


## Overview

This project develops and evaluates machine learning models to predict stroke occurrences based on health and demographic data.

## Data

- **Entries:** 5110
- **Features:** Age, BMI, Hypertension, Heart Disease, Smoking Status, etc.
- **Target:** `stroke` (1 = Stroke, 0 = No Stroke)

## Objectives

- Predict stroke based on health data.
- Compare model performance using accuracy, precision, recall, and F1-score.

## Data Preprocessing

- **Missing Values:** Imputed BMI with median.
- **Encoding:** One-hot encoded categorical variables.
- **Scaling:** Applied `StandardScaler` to numerical features.
- **Imbalance:** Used SMOTE and random undersampling.
- **Split:** 70/30 train-test ratio.

## Models Trained

- Naive Bayes
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Random Forest
- Support Vector Machine (SVM)
- Stacking Classifier

## Evaluation

| Model               | Accuracy | Precision | Recall | F1-Score |
|---------------------|----------|-----------|--------|----------|
| KNN                 | 88.58%   | 0.821     | 0.980  | 0.894    |
| Logistic Regression | 78.16%   | 0.754     | 0.823  | 0.787    |
| Random Forest       | 97.02%   | 0.985     | 0.954  | 0.969    |
| SVM                 | 77.51%   | 0.744     | 0.825  | 0.782    |
| Stacking            | 97.12%   | 0.977     | 0.964  | 0.970    |

## Key Insights

- **Top Performers:** Random Forest and Stacking Classifier show the highest accuracy and F1-score.
- **KNN:** High recall, useful for minimizing false negatives.

## Recommendations

- **Data Collection:** More data could enhance model performance.
- **Feature Engineering:** Include additional features like physical activity or family history.

## Conclusion

Random Forest and Stacking Classifier are recommended for stroke prediction, balancing precision and recall. Further improvements could involve additional data and advanced model tuning.
