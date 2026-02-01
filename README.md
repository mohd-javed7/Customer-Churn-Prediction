## Final Model Summary

- Both Logistic Regression and Decision Tree models identify a similar number of churn customers, achieving comparable recall (~0.60).
- The Decision Tree produces **significantly fewer false positives** compared to Logistic Regression (12 vs 107), while maintaining similar churn detection capability.
- As a result, the Decision Tree achieves **much higher precision** for the churn class (0.80 vs 0.31), meaning far fewer loyal customers are incorrectly flagged as churners.
- This leads to a **substantially lower operational cost**, as fewer unnecessary retention actions are triggered.
- Given its superior precision, strong recall, and higher ROC-AUC, the **Decision Tree is selected as the final model** for churn prediction.


## Business Interpretation

The final Decision Tree model enables proactive churn prevention by accurately identifying customers at risk of leaving while minimizing unnecessary interventions. This balance allows the business to allocate retention resources more efficiently and focus efforts on customers most likely to churn.


## Limitations

- The model was trained on historical customer data and may not capture future behavioral shifts.
- A single Decision Tree, while interpretable, may be sensitive to data variations.

