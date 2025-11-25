# Kaggle-Predicting-Loan-Payback
Playground Series - Season 5, Episode 11

Used CatBoost and RandomForest on different variance of data preprocessing with RandomSearch and GridSearch tuning.  
**Best score: ROC-AUC 0.92349; CatBoost with hyperparameter tuning and StandardScaler/Label Encoding on dataset. (CB_params_y_sub.csv)**

### Data: https://drive.google.com/drive/folders/1i_EdfGUfGBr919q38HCFF9431vEGxI82?usp=sharing 
* train.csv/test.csv/sample_submission.csv
  
* .._params.joblib - the best parameters for the model and specific data after GridSearch
* \**without "_params"*\* - X_train, y_train, X_test, y_test and dictionary with preprocessing models (SMOTE, le_scaler, ohe_scaler, StandardScaler)
* ..._y_sub.joblib - y_test probabilities from different models for submission.
  * final_... - final experiment with CatBoost without iterations and SMOTE, log transformation, categorical data scalers. 
