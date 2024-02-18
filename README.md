# Credit Risk Analysis report

## Overview
The purpose of this project was to use machine learning in order to predict the loans that were considered healthy or risky for loans. The factors that were considered were the size of the loan, interest rate, borrower's income, debt to income ratio, the number of accounts the borrower held, total debt, and deragatory marks against the borrower.

The dataset provided was first split into a training(75%) and testing(25%) in order to ensure that the model was predicting the credit worthiness of borrowers accurately. A logistic regression model was used in order to generate accuracy results

We wanted to compare the results by using the original dataset using "LogisticRegression" from scikit-learn library, then using the resampled data with "RandomOverSampler" module from the imbalanced-learn library, and find whether a loan would be considered low or high risk. 

## Results
### Machine Learning Model 1
- The logistic regression model that used the original imbalanced dataset predicted healthy loans 100% of the time, and non-healthy loans with an 89% of the time, with an accuracy of 96%.
- Recall for safe accounts was 99% and 94% for risky accounts
- 18,655 loans were a true positive, and 100 were a false positive
- 583 accounts were a true negative, and 36 were false negatives

### Machine Learning Model 2
- The balanced model predicted healthy loans 100% of the time, and risky loan 91% of the time, with an accuracy rate of 99%.
- Recall for both risky and safe accounts was 99%
- 18,646 loans were a true positive, and 119 were false positives.
- 615 accounts were true negatives, and 4 were false negatives

## Summary
For this specific situation, the second model would be more fitting, as it's more important to predict high-risk loans, and the RandomSampler was more accurate at finding true risky accounts.
