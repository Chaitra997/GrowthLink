**README FILE FOR CUSTOMER CHURN PREDICTION**

**Project Title:** Customer Churn Prediction
### **Objective:** The objective of this project is to predict whether a customer will discontinue a subscription-based service. By analyzing historical data, the goal is to identify customers who are likely to leave and understand the key factors that contribute to their churn.
**Dataset:** Bank Customer Churn Prediction 

**A.  Dataset Preprocessing Steps:** 

1. Importing the dataset and checking for missing values.
2. Dropping non-informative columns such as RowNumber, CustomerId, and Surname.
3. One-hot encoding applied to categorical variables Geography and Gender.
4. Scaling the numeric features using StandardScaler.
5. Splitting the dataset into training and testing sets.

**B.  Models:**  Several classification models were trained and evaluated:

1. **Decision Tree**
2. **Random Forest**
3. **XGBoost**
4. **SVM** 
5. **CatBoost**
6. **Artificial Neural Network (ANN)**

**C.  Handling Class Imbalance & Hyperparameter Tuning:**

- **SMOTE** (Synthetic Minority Over-sampling Technique) was applied to handle the imbalance. 
- **GridSearchCV** was used for hyperparameter tuning to improve model performance.


**D.  Model Evaluation Metrics:**  The following metrics were used to evaluate the performance of each model:

1. Accuracy
2. Precision
3. Recall
4. F1-Score

Both **with and without SMOTE** versions were compared.

**E.  Feature Importance Analysis:** Feature importance was analyzed using:

1. Random Forest
2. XGBoost
3. CatBoost

Key insights included identifying the most influential features such as:

1. Credit Score
2. Age
3. Balance
4. Tenure
5. Number of Products
6. IsActiveMember

Less influential features like HasCrCard were dropped after evaluation.



**F. Outcome:**

- The models effectively identified customers likely to churn.
- Insights from feature importance helped understand churn behavior.
- Models were tuned and evaluated with balanced data for better generalization.

|Model |Accuracy (No smote)|Precision (No smote)|Accuracy(smote)|Precision(smote)|
| :- | :- | :- | :- | :- |
|Decision Tree|0\.7870|0\.461358|0\.7690|0\.432485|
|Random Forest|0\.8635|0\.734375|0\.8380|0\.584352|
|XGBoost|0\.8600|0\.696864|0\.8535|0\.639665|
|SVM|0\.8600|0\.775610|0\.7865|0\.472492|
|CatBoost|0\.8655|0\.727941|0\.8665|0\.690909|
|ANN|0\.8575|0\.688811|0\.8090|0\.510978|









