# Credit_Risk_Analysis

# Background
All around the world people borrow money to buy real estate, cars, start a business and get an education. Loans present a challenge for banks and other money lenders.  One hand there is generation of revenue with the interested collected, on the other hand there is a risk associated with it as the borrowers may not pay it back. Rise of technology such as Fintech can allow the use of machine learning by the banks to analyze risk as oppose to the traditional indicators such as income and etc.

## Purpose
The purpose of this analysis is to use various machine learning models to predict credit risk.  Python and SciKit-learn is used in assessment. Strengths and weaknesses of different machine learning models is also evaluated based on how well the model classifies and predicts data.

# Results

The different types of analysis performed and the results are as follows:

### Naive Random Oversampling
The following shows the results for Naive Random Oversampling:

![Image1]()
- Balanced accuracy score = 64.9%
- High risk precision = 1%
- Low risk precision = 100%
- High risk recall = 62%
- Low risk recall = 68%

### SMOTE Oversampling
The following shows the results for SMOTTE Random Oversampling:

![Image2]()
- Balanced accuracy score = 64.4%
- High risk precision = 1%
- Low risk precision = 100%
- High risk recall = 63%
- Low risk recall = 66%

### Undersampling
The following shows the results for Undersampling:

![Image3]()
- Balanced accuracy score = 52.15%
- High risk precision = 1%
- Low risk precision = 100%
- High risk recall = 63%
- Low risk recall = 41%

### Combination Sampling
The following shows the results for Combination Sampling:

![Image4]()
- Balanced accuracy score = 52.15%
- High risk precision = 1%
- Low risk precision = 100%
- High risk recall = 70%
- Low risk recall = 57%

### Balanced Random Forest Classifier
The following shows the results for Balanced Random Forest Classifier:

![Image5]()
- Balanced accuracy score = 78.8%
- High risk precision = 4%
- Low risk precision = 100%
- High risk recall = 67%
- Low risk recall = 91%

### Easy Ensemble Classifier
The following shows the results for Easy Ensemble Classifier:

![Image6]()
- Balanced accuracy score = 92.5%
- High risk precision = 7%
- Low risk precision = 100%
- High risk recall = 91%
- Low risk recall = 94%

# Summary
This analysis was done to attempt to find a model that would reduce the risk that the banks/lenders would take when evaluating whether to grant loans or not.  

It is important to find a model that would let the least amount of high-risk loans to go undetected.  The high-risk recall is the value to be considered for it.  The best model would have the highest value for the high-risk recall.  That model was found to be Easy Ensemble Classifier at 91%.

Looking at the data, the model that detects the greatest number of low-risk loans as high risk.  The low-risk recall values should be evaluated to get an understanding of this factor.  It is found that it again is Easy Ensemble Classifier model at 94%.

The balanced accuracy score is the considered to determine what model performs the best.  Again, Easy Ensemble Classifier is the model that performs at 92.5% followed by Balanced Random Forest Classifier at 78.8%.

# Recommendation
- Looking at the data, it is recommended that the Easy Ensemble Classifier model be used due to the highest values in high-risk recall value, low risk recall value as well as the highest balance accuracy score when compared to all other models.  The model also has a high-risk precision score of 7%, which again is the highest when compared to all other models.
