Credit Card Fraud Detection using XGBoost
This project aims to develop a machine learning model that can accurately identify fraudulent credit card transactions. The dataset used for this project is highly imbalanced, with the majority of transactions being non-fraudulent.

The project was completed using Python, and the following libraries were used:

pandas
numpy
scikit-learn
xgboost
matplotlib
Data
The dataset used in this project was obtained from Kaggle. It consists of 284,807 credit card transactions, of which 492 are fraudulent.

Data Preparation
The first step in the project was to perform exploratory data analysis on the dataset. The dataset was highly imbalanced, with the majority of transactions being non-fraudulent. To address this, two techniques were used:

Undersampling the majority class
Oversampling the minority class
Both techniques were tested, and it was found that undersampling produced better results.

Next, the dataset was preprocessed to prepare it for machine learning. Categorical variables were one-hot encoded, and the features were standardized using the StandardScaler class from scikit-learn.

Model Development
The model used for this project was XGBoost, a popular gradient boosting library. A default XGBoost classifier was used to create a baseline model. Hyperparameter tuning was performed using grid search and early stopping to improve model performance.

The final model achieved an F1 score of 0.75 on the test data.

Deployment
The final model can be deployed using various methods, such as:

Creating an API with Flask or Django
Deploying the model on a cloud-based platform, such as AWS or Google Cloud
Conclusion
In conclusion, this project demonstrated how to develop a machine learning model to detect fraudulent credit card transactions. By using XGBoost and undersampling, we were able to achieve a high F1 score on the test data. The model can be deployed using various methods, depending on the use case.

For more information, please refer to the Jupyter Notebook and blog post included in this repository.
