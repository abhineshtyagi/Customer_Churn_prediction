# Customer_Churn_prediction
What is Customer Churn?
Customer churn is defined as when customers or subscribers discontinue doing business with a firm or service.

Customers in the telecom industry can choose from a variety of service providers and actively switch from one to the next. The telecommunications business has an annual churn rate of 15-25 percent in this highly competitive market.

Individualized customer retention is tough because most firms have a large number of customers and can't afford to devote much time to each of them. The costs would be too great, outweighing the additional revenue. However, if a corporation could forecast which customers are likely to leave ahead of time, it could focus customer retention efforts only on these "high risk" clients. The ultimate goal is to expand its coverage area and retrieve more customers loyalty. The core to succeed in this market lies in the customer itself.

Customer churn is a critical metric because it is much less expensive to retain existing customers than it is to acquire new customers.

To detect early signs of potential churn, one must first develop a holistic view of the customers and their interactions across numerous channels.As a result, by addressing churn, these businesses may not only preserve their market position, but also grow and thrive. More customers they have in their network, the lower the cost of initiation and the larger the profit. As a result, the company's key focus for success is reducing client attrition and implementing effective retention strategy.
# Objectives:
-Analysing the data in terms of various features responsible for customer Churn
-Finding a most suited machine learning model for correct classification of Churn and non churn customers.
# Some EDA part :

# 1.Churn Distribution
![image](https://github.com/user-attachments/assets/885d2e8d-8ced-4a65-84bd-4d5aca47143c)

# 2.Customer Contract Distribution vs Churn ( group Bar)
![image](https://github.com/user-attachments/assets/626c82a9-696b-435b-b29e-7da5273c2ab4)
# 3.Payment Method distribution vs Churn  (stacked Bar)
![image](https://github.com/user-attachments/assets/f1c3e51d-0b43-48bd-a4e2-ba1b9578f281)

# 4.Churn Distribution w.r.t Senior citizen
![image](https://github.com/user-attachments/assets/a737a83f-4673-4c72-8204-41623b17e371)

# Data preprocessing
-Label encoding for categorical Features 
-Apply SMOTE to balace the target data training dataset

# Model selection 

Training Decision Tree with default parameters
Decision Tree cross-validation accuracy : 0.78

----------------------------------------------------------------------
Training Random Forest with default parameters
Random Forest cross-validation accuracy : 0.84

----------------------------------------------------------------------
Training XGBoost with default parameters
XGBoost cross-validation accuracy : 0.81
**( "Among the models trained with default parameters, Random Forest achieved the highest cross-validation accuracy of 0.84, outperforming Decision Tree (0.78) and XGBoost (0.81).
Hence, Random Forest was selected as the baseline model for further tuning and evaluation.")**

# Model Training & Evaluation

With RandomForest Classifier  Achieving : Accuracy Score :
 0.7785663591199432
Confusion matrix:
 [[878 158]
 [154 219]]
Classfication Report :
               precision    recall  f1-score   support

           0       0.85      0.85      0.85      1036
           1       0.58      0.59      0.58       373

    accuracy                           0.78      1409
   macro avg       0.72      0.72      0.72      1409
weighted avg       0.78      0.78      0.78      1409

# Optimization 

Hyperparameter Tuning methods to improve the accuracy further 
Accuracy Score :
 0.7814052519517388
Confusion matrix:
 [[872 164]
 [144 229]]
Classfication Report :
               precision    recall  f1-score   support

           0       0.86      0.84      0.85      1036
           1       0.58      0.61      0.60       373

    accuracy                           0.78      1409
   macro avg       0.72      0.73      0.72      1409
weighted avg       0.79      0.78      0.78      1409





