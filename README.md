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

# Summary
