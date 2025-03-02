# credit-risk-classification

**README: Credit Risk Analysis Report**
**1. An overview of the analysis:** This analysis aims to build a machine learning model to classify loans as either healthy (0) or high-risk (1). The goal is to help financial institutions make informed decisions by accurately identifying high-risk loans, thereby minimizing potential losses. The dataset used for this analysis contains features related to loan applications, and the target variable is the loan status (loan_status).
A logistic regression model was trained and evaluated to predict loan status. The model's performance was assessed using metrics such as accuracy, precision, recall, and F1-score.

**2. The Results:**

 **Performance on Class 0 (Healthy Loan):**
•	Precision: 1.00 (100%): This means that 100% of the loans predicted as healthy There are no false positives for this class.
•	Recall: 1.00 (100%): This means that 100% of the actual healthy loans are correctly identified by the model. There are no false negatives for this class.
•	F1-Score: 1.00 (100%): A score of 1.00 indicates perfect performance for this class.
Conclusion: The model performs perfectly in predicting healthy loans. It correctly identifies all healthy loans without any errors.

**Performance on Class 1 (High-Risk Loan):**
•	Precision: 0.87 (87%): This means that 87% of the loans predicted as high-risk (1) are actually high-risk. The remaining 13% are false positives (loans predicted as high-risk but are actually healthy).
•	Recall: 0.95 (95%): This means that 95% of the actual high-risk loans are correctly identified by the model. The remaining 5% are false negatives (loans predicted as healthy but are actually high-risk).
•	F1-Score: 0.91 (91%): The F1-score is high, indicating a good balance between precision and recall for this class
Conclusion: The model performs very well in predicting high-risk loans, though there is a small trade-off between precision and recall. It correctly identifies 95% of high-risk loans, but there is a 13% chance that a loan predicted as high-risk is actually healthy.

**Overall Performance:**
•	Accuracy: 0.99 (99%): This means that 99% of all predictions (both healthy and high-risk loans) are correct.
•	Macro Avg: 0.94 precision, 0.97 recall, 0.95 F1-score: This is the unweighted average of the metrics for both classes. It shows that the model performs well across both classes, even though Class 1 has fewer samples.
•	Weighted Avg: 0.99 precision, 0.99 recall, 0.99 F1-score: This is the weighted average of the metrics, weighted by the number of samples in each class. Since Class 0 dominates the dataset, the weighted average is heavily influenced by its performance.

**3. A Summary:**
I recommend this model for use by the company because:
•	It achieves high overall accuracy (99%), making it a reliable tool for loan classification.
•	It performs exceptionally well on healthy loans, which constitute the majority of the dataset.
•	It demonstrates strong recall (95%) for high-risk loans, ensuring that most high-risk loans are correctly identified, which is critical for minimizing financial losses.
The logistic regression model performs best because it achieves a strong balance between precision and recall for both classes, with near-perfect accuracy. However, the importance of predicting 1s versus 0s depends on the business problem:
•	If minimizing defaults is the priority, focus on high recall for high-risk loans.
•	If maximizing revenue is the priority, focus on high precision for healthy loans.
In this case, the model's strong performance in both areas makes it a reliable choice for loan classification.
