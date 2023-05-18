# Credit Card Fraud Detection
The Credit Card Fraud Detection Problem includes modeling past credit card transactions with the knowledge of the ones that turned out to be fraud. So,this system is used to identify whether a new transaction is fraudulent or not. Our aim here is to detect 100% of the fraudulent transactions while minimizing the incorrect fraud classifications.

# For Dataset:-
https://www.kaggle.com/mlg-ulb/creditcardfraud


# about

The provided code is an example of anomaly detection in a dataset using two outlier detection algorithms: Isolation Forest and Local Outlier Factor. Here's a breakdown of what the code does:

1. Importing the required packages: The necessary libraries are imported, including numpy, pandas, matplotlib.pyplot, seaborn, sys, and scipy.

2. Loading the dataset: The dataset is loaded using pandas from a file specified by the "LOCATION OF THE FILE" placeholder.

3. Dataset exploration:
   - Printing the column names: The names of the columns in the dataset are printed.
   - Printing the shape of the data: The dimensions (number of rows and columns) of the data are printed.
   - Printing data statistics: Summary statistics of the dataset are printed, including count, mean, min, max, etc.

4. Plotting histograms: Histograms for each parameter in the dataset are plotted using the `hist` function from pandas. The histograms visualize the distribution of values for each parameter.

5. Determining the number of fraud cases: The code calculates the fraction of fraud cases in the dataset by dividing the number of fraud instances (Class = 1) by the number of valid instances (Class = 0). The result is stored in the `outlier_fraction` variable.

6. Printing the number of fraud cases and valid transactions: The code prints the number of fraud cases and valid transactions in the dataset.

7. Correlation matrix: The code computes the correlation matrix of the dataset using the `corr` function from pandas. It visualizes the correlation matrix as a heatmap using seaborn's `heatmap` function.

8. Data preprocessing:
   - Getting the columns from the DataFrame: All the column names from the dataset are stored in the `columns` variable.
   - Filtering unwanted columns: The code removes the "Class" column from the list of columns, as it is the target variable.
   - Splitting into features and target: The features (X) and target (Y) variables are separated from the dataset.

9. Printing the shapes of X and Y: The code prints the shapes (dimensions) of the feature matrix (X) and target vector (Y).

10. Importing necessary libraries: The code imports additional libraries required for classification evaluation, including `classification_report` and `accuracy_score` from sklearn.metrics, `IsolationForest` from sklearn.ensemble, and `LocalOutlierFactor` from sklearn.neighbors.

11. Defining random state: The variable `state` is set to 1, which will be used as the random state for the outlier detection algorithms.

12. Defining outlier detection tools: Two outlier detection algorithms, Isolation Forest and Local Outlier Factor, are defined as dictionary entries in the `classifiers` dictionary.

13. Plotting the number of errors: For each outlier detection algorithm, the code fits the data and predicts the outliers. It then compares the predicted outliers with the actual class labels (fraud or valid) to calculate the number of errors. The accuracy score and classification report are also printed.

The code seems to be an implementation of anomaly detection using Isolation Forest and Local Outlier Factor algorithms, but without the actual dataset or file location, it's difficult to provide more specific information about the results or potential improvements.
