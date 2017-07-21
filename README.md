# DC_Water_Pipeline
Prediction on water main break in DC water data

(1) Feature Tranformation: Converted the categorical values into numerical vlaues
    a. Creating Dummy Variables: For those columns that have several levels or categories, we assigned dummy variables to them
    b. Ordinal Data: Assigned 3 to "High",2 to "Moderate", and 1 to "Low" in those features.
    
(2) Feature Selection: 
    a. RFE
    
    b. Random Forest
    
    c. Correlation Matrix
    
(3) Evaluation of Machine Learning Models:
    Since we were dealing with imbalance data, evaulating models based on model accuarcy would lead to some problems and the results are misleading. Therefore, we can apply some resampling methods for making dataset more balanced (e.g SMOTE Over-Sampling or Under-Sampling). 
    In addition, we should use other metrics to evaluate the performance of models, such as K-fold cross-evaluation, confusion matix, precision rate, recall, and F-1 score, instead of using a single metric. In our case, we employed "Precision" as our model assessment metric. 
    For machine model development, we employed Random Forest, K-NN, Logistics Regression, SVM, Gradient Boosting Decision Tree, and ADA boosting. In addition, we also conducted parameters tunning in Random Forest. The results showed that "Gradient Boosting Decision Tree" with highest precision rate against other models.
    
