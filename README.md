# Machine Learning Churn Prediction

Churn is a very common problem for many companies, so to improve my machine learning skills, doing this complete project is of great help to get experience in real cases.

This notebook follows a step-by-step process to train the best possible model to solve the churn problem of a telecommunications company.

After receiving 4 dataframes with different data about the company's customers, makes a brief analysis of each of the dataframes, and then merges them into a single dataframe, then performs extensive EDA, identifies patterns of customers who are experiencing churn, and cleans the data to remove inconsistencies.

With the information acquired, perform feature engineering, transform the Yes or No columns into binary columns of 1 and 0, and do the encoding of the categorical variables.

To achieve at the best possible model, create a pipeline with several models using cross validation, plot the ROC curve and the confusion matrix, and analyze the AUC-ROC score of each of the models.

Then select the 3 best models to proceed with hyperparameter tuning, and then test them on the test set.

With the final model chosen, analyze it extensively with the shap library and using bootstrapping.