**Linear Regression**

**AI in Robotics**

**Task 1**

*Name: Doha Eid Ali*

*Sec: 1*

*BN: 49*

**Introduction**:

This code performs linear regression on the "insurance.csv" dataset to predict insurance charges based on several features. Given a dataset containing information about individuals' characteristics (such as age, gender, BMI, number of children, smoking status, and region), the task is to build a regression model that can predict the insurance charges for new individuals based on their characteristics.

**Dataset**:

It contains information about individuals' insurance charges based on various factors or features. Here's a breakdown of the columns in the dataset:

-   age: Age of the individual (numeric).
-   sex: Gender of the individual. It is encoded as 'male' or 'female' (categorical).
-   bmi: Body mass index (numeric).
-   children: Number of children the individual has (numeric).
-   smoker: Whether the individual is a smoker or not. It is encoded as 'yes' or 'no' (categorical).
-   region: The region where the individual resides. It is encoded as 'southwest', 'southeast', 'northwest', or 'northeast' (categorical).
-   charges: Insurance charges incurred by the individual (numeric).

**Packages**:

The code utilizes several Python packages to perform various tasks. Here are the packages used in the code.

-   numpy (imported as np): It provides support for handling arrays, mathematical operations, and linear algebra calculations.
-   pandas (imported as pd): It provides data structures (e.g., DataFrame) to efficiently work with structured data and offers various functions for data preprocessing and exploration.
-   sklearn.model_selection: It includes the train_test_split function used to split the dataset into training and test sets.
-   matplotlib.pyplot (imported as plt): A plotting library that provides a MATLAB-like interface for creating visualizations.

**Code overview:**

1.  Model using scikit learn library (Model 1):
-   Import data (insurance dataset).
-   Data preparation (convert string data to numerical data, split data as target and train data, and split data as train and test data).
-   Call linear regression function from sklrean library to train model.
-   Predict test data.
-   Evaluate model.
1.  Model using scratch Python code to implement linear regression function (Model 2):
-   Implement function of linear regression using equation of LR (Y_i=f(X_i, \\beta)+e_i).
-   Predict function that uses y_predict=w.x+b
-   Normalize function to normalize input features X.
-   Denormalization function to cancel normalization effect to represent actual data.
-   R2 score function to evaluate the model.
-   Mean square error function to evaluate the model.
-   Import data.
-   Data preparation (convert string data to numerical data, split data as target and train data, and split data as train and test data).
-   Split inputs and target X, Y.
-   Normalize input feature X.
-   Set learning rate and number of iterations.
-   Calculate weights and biases from linear regression function.
-   Evaluate model.
-   Denormalization to represent the actual values.
-   Plotting data with line of LR.

**Compare results:**

1.  ![](media/018628ea8aa1b1f55d0281c4eb8832a5.tmp)Model using scikit learn library (Model 1):
-   R2 score : 0.79
-   MSE: 0.33
1.  ![](media/7d0d9f2a52fd8933def833212cef9dd2.tmp)Model using scratch Python code to implement linear regression function (Model 2):
-   R2 score: 0.74
-   MSE: 0.26
-   **Results from two models that:**
-   Based on the provided results, we can see that the models built using the scikit-learn library (Model 1) outperformed the model implemented from scratch using Python code (Model 2) in terms of both R-squared score and mean squared error (MSE). A higher R-squared score indicates that the scikit-learn model (Model 1) explains more of the variance in the data compared to the scratch implementation (Model 2). Similarly, a lower MSE value indicates that the scikit-learn model has smaller errors on average when predicting the target variable.
-   Scikit-learn linear regression: Easy to use, optimized, and offers a wide range of functionalities but Limited customization and less transparency in implementation details.
-   Scratch Python linear regression: Provides understanding, flexibility, and customization options. Requires more code, may be less optimized, and lacks integration with other tools
