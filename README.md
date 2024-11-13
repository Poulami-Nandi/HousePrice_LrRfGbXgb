# HousePrice_LrRfGbXgb

House Prices - Advanced Regression Techniques
This project aims to predict the final sale prices of residential homes in Ames, Iowa, based on various features, using machine learning regression techniques. This dataset is provided as part of the Kaggle competition.

Project Structure
Data Exploration and Visualization: Understanding the data, visualizing distributions, and identifying key features.
Data Preprocessing: Handling missing values, encoding categorical variables, and scaling numerical features.
Feature Engineering: Creating new features to improve model performance.
Model Training and Evaluation: Training multiple models, calculating their RMSE scores, and selecting the best model.
Final Prediction and Submission: Generating predictions for the test set and saving the results in a submission file.
Data
The project uses two datasets:

train.csv: Contains the training data with SalePrice as the target variable.
test.csv: Contains the test data for which we will predict SalePrice.
Preprocessing
Handling Missing Values: Imputed missing values with median or most frequent values, depending on the feature type.
Encoding Categorical Variables: Used LabelEncoder for categorical variables to ensure compatibility with regression models.
Feature Engineering: Added new features like TotalSF (total square footage) to capture property size.
Models Used and RMSE Scores
Model	RMSE
Linear Regression	0.1447
Random Forest Regressor	0.1352
Gradient Boosting	0.1278
XGBoost	0.1221
Selected Model: XGBoost
The XGBoost model provided the lowest RMSE on the validation set, so it was selected for generating predictions on the test set.

Results and Submission
The final predictions were generated using the XGBoost model and saved to submission.csv for submission to the competition.

How to Run the Project
Install Required Libraries:

Copy code
pip install pandas numpy scikit-learn xgboost matplotlib seaborn
Execute the Notebook: Open the Jupyter notebook provided (House_Prices_Solution.ipynb) and run each cell sequentially to preprocess the data, train the models, and generate predictions.

