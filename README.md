# Module 12 Report Template

## Overview of the Analysis

Purpose of the Analysis: The purpose of this model was to precict and analyze the loan risk of potential borrowers. As a result, this would allow the lending company to make better lending decisions. This model was created using a dataset containing historical lending activity from a lending services company.

Financial Information: The dataset contained several variables that contribute to the riskiness of borrowers. These included loan size, interest rates, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and the total amount of debt. The loan status variable—a binary variable indicating whether a person should be granted a loan or not—was the target variable we used in our predictions.

Stages of the Machine Learning Process: First, the data were imported and converted into a Pandas DataFrame. Second, the target variable (the variable being predicted by the model) was assigned to the borrowers' loan status. After the target variable was created and assigned, the data were split into ‘training’ and ‘testing’ groups. The ‘train’ set of data was the data used to train the model into recognizing the patterns, and the ‘test’ set was used to test the accuracy of the training. We allocated 20% of the data to the ‘test’ set. After the data were trained, it was fitted into the model using a logistic regression analysis. Since loan status is a binary variable, we selected a logistic regression. After the model was created, its performance was evaluated by using a balanced accuracy score, confusion matrix, and a classification report.


## Results

Accuracy:
* The balanced accuracy score of the model was 0.9521. This means that the logistic regression correctly predicted 95.21% of the actual loan status values in the dataset.

Precision:
* Precision for the high-risk loans is 0.85, meaning that it will correctly predict a high-risk loan 85% of the time.
* Precision for the low-risk loans is 1.00, meaning that it will correctly predict a low-risk loan 100% of the time.

Recall:
* Recall for the low-risk loans is 0.99, meaning that the model correctly identifies 99% of the actual low-risk loans.
* Recall for the high-risk loans is 0.91, meaning that the model correctly identifies 91% of the actual high-risk loans.

## Summary and Recommendations

The model's performance is strong, as it possesses a balanced accuracy score of 95.21%, high precision scores for both low and high-risk loans, and excellent recall metrics. The model is particularly effective in correctly identifying low-risk loans with a precision of 1.00 and a high recall of 0.99.
The model's performance depends on what it's being used for. In order to minimize lending to high-risk borrowers, the model performs well—as demonstrated by a precision of 0.85 and a recall of 0.91. However, the model is more accurate when maximizing lending to low-risk borrowers—as demonstrated by a precision of 1.00 and a recall of 0.99.

## Outside Assistance

Tutor Simon Rennocks assisted with the development of the logic and the syntax of the python code in the Jupyter Notebook file and assisted with the application of machine learning concepts for the written report.
