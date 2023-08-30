#  Background


In this Challenge various techniques were used to train and evaluate a model based on loan risk. The dataset consists of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

#  Instructions


1. Split the Data into Training and Testing Sets


-  Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.

-  Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.

NOTE
A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.

- Split the data into training and testing datasets by using train_test_split.

2. Create a Logistic Regression Model with the Original Data


- Fit a logistic regression model by using the training data (X_train and y_train).

- Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.

Evaluate the model’s performance by doing the following:

- Generate a confusion matrix.

- Print the classification report.

Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

#  Results

The logistic regression model was 95% accurate according to the balanced accuracy score. However, the confusion matrix shows that the data is very imbalanced. There are a lot more healthy loans than there are high risk loans. The classification report reveals that the model is 100% accurate predicting healthy loans but only 85% accurate when predicting high-risk loans.

![Screenshot 2023-08-30 081557](https://github.com/Jeremy-Mallory/credit-risk-classification/assets/122320256/ffd16c68-59b5-4542-8bf1-b9d589b90644)


![Screenshot 2023-08-30 080403](https://github.com/Jeremy-Mallory/credit-risk-classification/assets/122320256/9d7d05c2-3661-44dc-88da-6a4653e74f46)


To rectify this issue, a random over-sampler was used in the next iteration of the model.


![Screenshot 2023-08-30 080556](https://github.com/Jeremy-Mallory/credit-risk-classification/assets/122320256/8d780477-fcd9-48af-a223-02a73a5bab9c)


The model fit with oversampled data was 99% accurate as opposed to 95% previously. The oversampled model seems to be better at correctly classifying high risk loans as evidenced by the recall score which was originally 0.91, now 0.99.


![Screenshot 2023-08-30 081625](https://github.com/Jeremy-Mallory/credit-risk-classification/assets/122320256/c29b2df2-8e5c-4889-b729-7f4e57261c3f)


![Screenshot 2023-08-30 080455](https://github.com/Jeremy-Mallory/credit-risk-classification/assets/122320256/2608ad7f-4d55-4a41-9a62-7bcc6ac2e51e)

