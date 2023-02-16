# Module-18_assignment
## Objective: Predicting loan status based on dataset
### Purpose: To compare 6 different machine learning models and their ability to correctly predict loan status
### Definitions:
 - Balanced accuracy score = This corresponds to the average of the true positive rate and true negative rate
 - Precision = This corresponds to the ability of the model to predict actually positive cases out of all its predicted positive cases
 - Recall = This corresponds to the ability of the model to correctly predict positive cases out of all the actual positive cases

Note: The balanced accuracy score and the recall appear similar. However, we derive the recall from the imbalanced report which takes into account the imbalance between the high risk and low risk classes, whereas the balanced accuracy average is simply derived by dividing the TPR and TNR by 2.

What is useful about having both measurements is that it indicates to us the impact of the class imbalance on the model's performance.

### Model 1: Using Random oversampling
Here are some key features of this model:
 - Balanced accuracy score = 0.67, means the model correctly predicts the loan status 67% of the time.
 - Precision average = 0.99 (1 for low risk, 0.01 for high risk) this means that in nearly all cases when the model predicts positive it's actually positive. In fact this is always true when it predicts low risk loans. However, for high risk loans it almost never predicts it accurately.
 - Recall = 0.61 (0.60 for low risk, 0.74 for high risk) this means that the model on average predicts 61% of the loan statuses correctly.
 
 
 ### Model 2: SMOTE oversampling
Here are some key features of this model:
 - Balanced accuracy score = 0.66, means the model correctly predicts the loan status 66% of the time.
 - Precision = 0.99 (1 for low risk, 0.01 for high risk) this means that in nearly all cases when the model predicts positive it's actually positive. In fact this is always true when it predicts low risk loans. However, for high risk loans it almost never predicts it accurately.
 - Recall = 0.69 (0.69 for low risk, 0.63 for high risk) this means that the model on average predicts 63% of the loan statuses correctly.
 
 
 ### Model 3: Undersampling
Here are some key features of this model:
 - Balanced accuracy score = 0.54, means the model correctly predicts the loan status 54% of the time.
 - Precision = 0.99 (1 for low risk, 0.01 for high risk) this means that in nearly all cases when the model predicts positive it's actually positive. In fact this is always true when it predicts low risk loans. However, for high risk loans it almost never predicts it accurately.
 - Recall = 0.4 (0.4 for low risk, 0.69 for high risk) this means that the model on average predicts 40% of the loan statuses correctly.
 
 
 ### Model 4: SMOTEEN
Here are some key features of this model:
 - Balanced accuracy score = 0.64, means the model correctly predicts the loan status 64% of the time.
 - Precision = (1 for low risk, 0.01 for high risk) this means that in nearly all cases when the model predicts positive it's actually positive. In fact this is always true when it predicts low risk loans. However, for high risk loans it almost never predicts it accurately.
 - Recall = 0.57 (0.57 for low risk, 0.72 for high risk) this means the model on average predicts 57% of the loan statuses correctly.
 
 
 ### Model 5: Balanced Random Forest Classifier
Here are some key features of this model:
 - Balanced accuracy score = 0.79, means the model correctly predicts the loan status 79% of the time.
 - Precision = 0.99 (1 for low risk, 0.03 for high risk) this means that in nearly all cases when the model predicts positive it's actually positive. In fact this is always true when it predicts low risk loans. However, for high risk loans it almost never predicts it accurately.
 - Recall = 0.87 (0.70 for low risk, 0.87 for high risk) this means that the model on average predicts 87% of the loan statuses correctly.
 
 
 ### Model 6: Easy Ensemble Classifier
Here are some key features of this model:
 - Balanced accuracy score = 0.93, means the model correctly predicts the loan status 93% of the time.
 - Precision = 0.99 (1 for low risk, 0.09 for high risk) this means that in nearly all cases when the model predicts positive it's actually positive. In fact this is always true when it predicts low risk loans. However, for high risk loans it almost never predicts it accurately.
 - Recall = 0.94 (0.94 for low risk, 0.92 for high risk) this means that the model on average predicts 94% of the loan statuses correctly.
 
 
 ### Conclusion: The Easy Ensemble Classifier model is the most accurate in predicting loan status based on the seen variables.
 
