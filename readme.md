## Credit Card Fraud Detection using XGBoost

### Acknowledgements

The credit card fraud dataset was obtained from [Kaggle](https://www.kaggle.com/datasets/mishra5001/credit-card)


### Project Overview
The goal of this project is to develop a machine learning model to detect credit card fraud. The dataset used in this project is highly imbalanced, with a very small percentage of fraudulent transactions. The project involves data cleaning, exploratory data analysis, feature engineering, and modeling using XGBoost classifier. Hyperparameter tuning was performed using grid search to increase the F1 score from 0.72 to 0.97.

The project was completed using Python, and the following libraries were used:

pandas
numpy
matplotlib
scikit-learn
xgboost


The dataset used in this project was obtained from Kaggle. It consists of 284,807 credit card transactions, of which 492 are fraudulent.

### Data Preparation
The first step in the project was to perform exploratory data analysis on the dataset. The dataset was highly imbalanced, with the majority of transactions being non-fraudulent. To address this, two techniques were used:

Undersampling the majority class
Oversampling the minority class

Both techniques were tested, and it was found that undersampling produced better results.

Principal Component Analysis was applied for dimensionality reduction. I found 24 PC's to be the optimal number for analysis.

Next, the dataset was preprocessed to prepare it for machine learning. Categorical variables were one-hot encoded, and the features were standardized using the StandardScaler class from scikit-learn.

### Model Development
The model used for this project was XGBoost, a popular gradient boosting library. A default XGBoost classifier was used to create a baseline model. Hyperparameter tuning was performed using grid search and early stopping to improve model performance.

The final model achieved an F1 score of 0.96 on the test data.


### Conclusion
In conclusion, this project demonstrated how to develop a machine learning model to detect fraudulent credit card transactions. By using XGBoost and undersampling, we were able to achieve a high F1 score on the test data.

For more information, please refer to the Jupyter Notebook and blog post included in this repository.

### Future Work

Some potential next steps to improve the project include:

Trying other classification algorithms such as Random Forest or SVM
Experimenting with different feature engineering techniques
Using other methods to address class imbalance such as oversampling or SMOTE
Deploy the model 
