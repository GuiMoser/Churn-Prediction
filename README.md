# Machine Learning Churn Prediction

## Project Description
Churn is a very common problem for many companies, so to improve my machine learning skills, doing this complete project is of great help to get experience in real cases.

This notebook follows a step-by-step process to train the best possible model to solve the churn problem of a telecommunications company.

After receiving 4 dataframes with different data about the company's customers, makes a brief analysis of each of the dataframes, and then merges them into a single dataframe, then performs extensive EDA, identifies patterns of customers who are experiencing churn, and cleans the data to remove inconsistencies.

With the information acquired, perform feature engineering, transform the Yes or No columns into binary columns of 1 and 0, and do the encoding of the categorical variables.

To achieve at the best possible model, create a pipeline with several models using cross validation, plot the ROC curve and the confusion matrix, and analyze the AUC-ROC score of each of the models.

Then select the 3 best models to proceed with hyperparameter tuning, and then test them on the test set.

With the final model chosen, analyze it extensively with the shap library to analyze the feature importance and uses bootstrapping to see the confidence interval.

## Objectives
- Perform exploratory data analysis.
- Identify patterns of customers who are experiencing churn.
- Clean the data to remove inconsistencies.
- Perform feature engineering.
- Transform the Yes or No columns into binary columns of 1 and 0.
- Do the encoding of the categorical variables.
- Create a pipeline with several models using cross validation.
- Plot the ROC curve and the confusion matrix.
- Analyze the AUC-ROC score of each of the models.
- Select the 3 best models to proceed with hyperparameter tuning.
- Test them on the test set.

## Tools and Libs used
- Python: Main language used for analysis.
- Pandas: Library for data manipulation and analysis.
- NumPy: Library for numerical operations.
- Matplotlib and Seaborn: Libraries for data visualization.
- Scikit-learn: Library for machine learning.
- Optuna: Library for hyperparameter tuning.
- LightGBM, XGBoost e Catboost: Libs for gradient boosting.
- Shap: library to analyze the feature importance
- Bootstrapping: Library for confidence interval.

## Methodology
#### EDA
- Brief analysis of each of the dataframes.
- Merge the 4 dataframes using customer_id as the base.
- Perform EDA on this dataframe.
    - Clean the data and remove inconsistencies.
    - Visualize the data and understand the variables.
    - Identify patterns of customers who suffer from churn.
#### Feature Engineering
- Perform feature engineering.
#### Model Training
- Split the data into training and testing.
    - Transform the Yes or No columns into binary columns of 1 and 0.
    - Perform encoding of the categorical variables.
- Use AUC-ROC metric.
    - Great metric for churn problems.
- Train several classification models on the validation set.
    - Create pipelines of the models.
    - Perform Cross-Validation
    - Plot ROC curve and confusion matrix for the models.
    - Evaluate the model based on the AUC-ROC metric.
#### Model Evaluation
- Choose the best models to proceed.
    - Perform hyperparameter tuning on these models. 
    - Train the best models on the test set.
- Analyze the best model extensively.

## Conclusions
We performed the entire step-by-step process for training the model. All inconveniences found were easily resolved during EDA, such as column conversion, creation of the target "churn" column as binary, encoding and scaling performed before training the tested models. With two main stages of the project, one of them being EDA, where we were able to understand the data and analyze possible causes for this problem, and hyperparameter tuning, where we ensured that the model obtained a high AUC score in the test set, as well as in the validation set to solve the problem we identified.

## Learnings
- Data analysis: Interpreting and extracting valuable insights from large volumes of data.
- Data cleaning: Identifying and correcting missing, duplicate, and anomalous values.
- Creating graphics: Using matplotlib and seaborn to visualize data in an intuitive and informative way.
- Data preprocessing: Preparing Data for analysis, including cleaning and treat the data.
- Use of libraries and tools: Practical application of various libraries and tools from the Python ecosystem, such as Pandas, Numpy, Sklearn, Matplotlib and Seaborn.
- Data visualization: Creating very detailed graphs and other types of visualizations to identify patterns and trends.
- Data-driven decision making: Using insights derived from data analysis to guide strategic decisions.
- Regression Models: Train and evaluate regression models.
- Model comparison: Compare models based on different metrics
- Pipeline: Process that manages the flow of data into and out of a machine learning model
- Feature selection: Selecting the best features to split between training, validation and testing.
- Feature engineering: Creating new features from existing ones.
- Hyperparameter tuning: Using Optuna to find the best hyperparameters for the models.
- Gradient Boosting: Using LightGBM, XGBoost and Catboost to train models.
- Model interpretation: Understanding the behavior of the models and the importance of the features.
- Bootstrapping: Resampling the data repeatedly drawing samples from a dataset with replacement.
- Cross-validation: Evaluating the performance of a model on unseen data.
