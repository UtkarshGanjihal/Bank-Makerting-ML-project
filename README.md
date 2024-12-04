# Bank-Makerting-ML-project
# Predicting Term Deposit Subscriptions Using Machine Learning

This project uses the Bank Marketing dataset to predict whether a client will subscribe to a term deposit. It includes data preprocessing, handling class imbalance, and training machine learning models to achieve competitive performance metrics.

## Key Features
- **Binary Classification:** Predicts customer subscription (`yes`/`no`).
- **Imbalanced Dataset Handling:** Applied SMOTE to balance the classes.
- **Model Evaluation:** Compared Logistic Regression, Random Forest, and XGBoost, optimizing for recall and AUC-ROC.

## Results
- **Best Model:** XGBoost with an adjusted threshold (AUC-ROC: 0.778).
- **Minority Class Recall:** Improved from 33% to 70% with threshold tuning.

## Tools and Techniques
- **Languages:** Python (pandas, NumPy, scikit-learn)
- **Models:** Logistic Regression, Random Forest, XGBoost
- **Techniques:** SMOTE, Hyperparameter Tuning, Threshold Adjustment
- **Visualization:** Matplotlib

## Performance Summary
| **Model**             | **Accuracy** | **F1 (Class 1)** | **Precision (Class 1)** | **Recall (Class 1)** | **AUC-ROC** |
|------------------------|--------------|------------------|-------------------------|----------------------|-------------|
| Logistic Regression    | 81%          | 0.42             | 0.32                   | 0.62                | 0.774       |
| Random Forest          | 79%          | 0.40             | 0.30                   | 0.61                | 0.765       |
| XGBoost (Threshold 0.5)| 82%          | 0.43             | 0.33                   | 0.62                | 0.778       |
| XGBoost (Threshold 0.4)| 72%          | 0.36             | 0.24                   | 0.70                | 0.778       |

## Instructions
1. Clone this repository.
2. Install the required libraries (`pip install -r requirements.txt`).
3. Run the notebook `bank_marketing_analysis.ipynb` to see the full implementation.
4. Evaluate models and test with custom thresholds.

## Dataset
The original dataset is derived from the **Bank Marketing Dataset** available on the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing).

## Author
[Utkarsh Ganjihal]([https://www.linkedin.com/in/utkarsh-ganjihal/])
