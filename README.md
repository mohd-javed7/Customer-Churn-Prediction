# Customer Churn Prediction

This project focuses on predicting customer churn using a structured and interpretable machine learning workflow. The goal is not only to build accurate models, but to make **data-driven decisions based on business impact**, particularly in handling class imbalance and model trade-offs.

## Problem Statement
Customer churn refers to customers discontinuing a service. Identifying customers at risk of churn allows businesses to take proactive retention actions. The challenge lies in handling **imbalanced data** and selecting a model that balances churn detection with operational cost.

## Approach
The project follows a complete end-to-end machine learning pipeline:

- Exploratory Data Analysis (EDA) to understand feature behavior and churn patterns  
- Feature preprocessing using `ColumnTransformer` and `Pipeline` to prevent data leakage  
- Baseline Logistic Regression model for interpretability  
- Handling class imbalance using:
  - Threshold tuning
  - Class weighting  
- Model evaluation using precision, recall, F1-score, ROC-AUC, and confusion matrices  
- Comparison between a linear model (Logistic Regression) and a non-linear model (Decision Tree)  
- Final model selection based on both performance metrics and business considerations  

## Key Findings
- Logistic Regression provided a strong interpretable baseline but struggled with false positives.
- A depth-limited Decision Tree achieved comparable recall while **significantly reducing false positives**.
- The Decision Tree offered a better balance between churn detection and operational efficiency.
- Based on confusion matrix analysis and ROC-AUC, the Decision Tree was selected as the final model.

## Final Model
- **Decision Tree Classifier (depth-limited)**
- Chosen for its higher precision, strong recall, and lower operational cost.

## Tools & Technologies
- Python
- pandas, NumPy
- scikit-learn
- Matplotlib / Seaborn

## Evaluation Metrics
- Precision, Recall, F1-score
- ROC-AUC
- Confusion Matrix

## Limitations
- Model trained on historical data may not capture future behavioral changes.
- A single Decision Tree can be sensitive to data variations.

## Future Work
- Experiment with ensemble models (Random Forest, Gradient Boosting).
- Incorporate explicit business cost functions.
- Monitor model performance for data drift and retraining needs.

---

This project emphasizes **model reasoning, interpretability, and business impact** over blind metric optimization.
