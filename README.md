# Project Overview & Analysis Report

The purpose of this project was to create a machine learning model that could correctly identity the creditworthiness of borrowers based on historical lending data. For the model, we used several features including: loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory remarks, and total debt. Borrowers loans were then categorized into one of two groups- healthy (0) or high-risk (1) using a Logistic Regression algorithm. 

## Results

* Model Results:
    * Precision: Healthy Loan- 100%, High-Risk- 85%
    * Recall: Healthy Loan- 99%, High-Risk- 91%
    * f1-Score: Healthy Loan- 100%, High-Risk- 88%
    * Datapoints: Healthy Loan- 18,765, High-Risk- 619
    * Overall Model Accuracy: 99% with 19,384 datapoints

## Summary

The logistic regression model does a near-perfect job of predicting healthy loans with a precision score of 100%, a recall score of 99% and an f-1 score of 100%. The model also does a very good job at predicting high-risk loans with a precision score of 85%, recall score of 91% and an f-1 score of 88%. The model does not do as well with high-risk loans, however taking into account the fact that there are significantly fewer high-risk loans to analyze, it is understandable that the model does not perform as well as it does for healthy loans. The weighted score of 99% across all features indicated that this is a very good model for use overall.

I would recommend using this model in order to determine the credit-worthiness of a specific borrower- especially if the model determines that the borrower's loan would be a "healthy" one. If the model classifies a particular borrower as "high-risk" I believe the model would be overall a good indicator, however perhaps getting an extra set of eyes on the data would be warranted because the model is not quite as good at determining "high-risk" loans. As "high-risk" loans are the most important loans to identify, a second verification process is not necessary, but I believe would provide greater confidence to the financial institution. 


## Source Data
- The data for this assignment was provided to us in the form of [lending_data.csv](./Resources/lending_data.csv).

## References
- The code written for this assignment was written using scikit-learn documentation, examples from class, class notes, examples from StackOverflow, ChatGPT, along with collaboration and help from my classmates, and tutors.
