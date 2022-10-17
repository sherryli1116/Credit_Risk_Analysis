# Credit_Risk_Analysis
## Overview of the analysis
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Credit card companies must evaluate new customer credit applications to assess the applicant's credit risk.

The goal of this project is to build a classification model that can predict if an applicant is likelky to have low or high credit risk. The credit card company can use this information to determine whether or not an applicant should be approved. We will employ different techniques to train and evaluate models with unbalanced classes and evaluate models using resampling. We will then evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results
- Accuracy Score：a measure of how likely a model is to label all predictions correctly.
- Preciscion： a classifier's ability to accurately label samples and minimize false positives or negatives.
- Recall： a classifier's ability to find all the positive or negative samples. In this scenario, the higher the recall, the less chance there is that a high risk applicant will be classified as low risk and vice versa.


## Summary
While resampling can attempt to address imbalance, it does not guarantee better results. In terms of this dataset, we find that the best overall model to use is the "Easy Ensemble AdaBoost Classifier" because not only does it have a high accuracy score, but it also has the best precision and sensitivity (recall) especially in terms of correctly identifying high-risk applicants. Therefore, we would reccomend using this model to predict credit risk.

The one downside to this model is a high false positive rate meaning that of the applicants that are predicted to be high risk, only a small amount of them will actually be high risk. In this scenario though, it is better for the model to have greater senstivity than precision because the credit card company would rather wrongly classify low risk applicants as high risk, than have high risk applicants classified as low risk thus approving them for a credit card or loan they are unable to repay. Also, the credit card company can further narrow down and examine these potential high risk individuals later on outside of the machine learning scope.
