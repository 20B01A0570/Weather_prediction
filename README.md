# Weather_prediction
PYTHON MODULES REQUIRED:
pandas: allows the user to perform various actions for manipulating a dataset.

numpy: it is an array-processing package and provides tools to work with data arrays.

train_test_split: it is a part of sklearn.model which helps in dividing the data for training and testing purposes.

RandomForestRegressor: capable of doing regression and classification of the data with the help of decision trees at training time.

**Procedure to develop the model for weather prediction**:
NOTE: The dataset used in this program is extracted from meteoblue.com

Dataset used: temps2.csv for the csv file.

1.First of all, we read the ‘.csv’ file containing the required dataset using ‘read_csv()’ function.
2.Now, to convert the categorical data to numerical data, we use ‘get_dummies()’ function.
3.To get the required column of the dataset on which we have to perform the training and testing, we use ‘iloc[]’ function.
4.To store the data to be processed separately, use ‘array()’ function of the numpy header file.
5.Now’s the time to divide our data for training and testing purposes.
We use train_test_split() function to achieve so.

The syntax of the function is:

train_test_split(X,y, train_size, test_data_size, random_state=1)

X,y: parameters of the dataset that are used to split

train_size: sets the size of the training set.

test_size: sets the size of testing data.

random_state: performs a random split.
6. Now, to perform regression and classification of the data so as to get the accurate result we use RandomForestRegressor().
The syntax of this function is:

RandomForestRegressor(n_estimators, random_state)

n_estimators: no. of decisions tress  in the training data.

7. Also, for better accuracy of the developed model, we use ‘fit()‘ function. This function trains the model using data examples and best matches the curvature of the given data points.

8. Now, to finally predict future values using the model, we should use ‘predict()‘ function which is in-built in pandas.

9. We print the predictions and also calculate and display the accuracy of our model.

