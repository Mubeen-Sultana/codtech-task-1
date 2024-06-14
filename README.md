Name: MUBEEN SULTANA
Company: CODTECH IT SOLUTIONS
ID: CT08PP699
Domain: DATA SCIENCE
Duration: MAY TO JUNE 2024
Mentor: SRAVANI GOUNI

TASK 1 - Exploratory Data Analysis (EDA) 

Overview of the Project

Project: Google Play Store - Exploratory Data Analysis (EDA) and Predictions using Random Forest
1. Introduction
The project focuses on performing exploratory data analysis (EDA) and building a machine learning model using a dataset from the Google Play Store. The goal is to understand the data, clean and preprocess it, and then build a predictive model to estimate app ratings based on various features.
2. Importing Libraries
To start, essential libraries are imported for handling data manipulation, visualization, and machine learning. This includes libraries such as numpy for numerical computations, pandas for data manipulation, matplotlib and seaborn for visualization, and libraries from sklearn for machine learning tasks.
3. Loading and Exploring Data
The dataset is loaded into a DataFrame using pandas. Initial exploration involves:
Displaying a sample of the data to understand its structure and contents.
Checking the dataset's dimensions to see how many rows and columns it contains.
Using data summary methods to get an overview of the data types and the number of non-null entries for each column.
Identifying missing values across the dataset, which is crucial for determining how to handle incomplete data.
4. Cleaning Data
Data cleaning is a critical step to ensure the dataset is suitable for analysis and modeling. This involves:
Size Conversion: Converting the Size column values from strings with 'M' (megabytes) and 'k' (kilobytes) suffixes into numerical values. Sizes in kilobytes are converted to megabytes or bytes, and sizes not specified are marked as missing.
Installations: Cleaning the Installs column by removing non-numeric characters and converting the values to numeric format.
Pricing: Cleaning the Price column by removing currency symbols and converting the values to numeric format.
Missing values in the Size column are filled with the mean size of the respective app category. Rows with missing sizes and ratings are removed to maintain the dataset's integrity.
5. Exploratory Data Analysis (EDA)
EDA involves generating summary statistics and visualizations to understand the dataset better. Key steps include:
Summary Statistics: Calculating descriptive statistics for numerical columns to understand the central tendency, dispersion, and overall distribution.
Distribution Analysis: Visualizing the distribution of key numerical features like Rating, Size, and Reviews using kernel density plots to see how these values spread across the dataset.
Categorical Analysis: Creating count plots for categorical variables such as Type, Content Rating, and Category to see the frequency distribution of different categories.
Category Ratings: Analyzing and visualizing the mean ratings of apps per category to identify which categories tend to have higher or lower ratings.
Correlation Analysis: Using regression plots to explore relationships between pairs of variables such as Reviews vs. Ratings, Price vs. Ratings, and Reviews vs. Size. This helps in identifying potential predictors for the target variable (ratings).
6. Data Preparation for Machine Learning
Preparing the data involves several key steps:
Feature Selection: Dropping columns that do not contribute numerically to the regression model, such as version and date columns.
Encoding Categorical Variables: Converting categorical variables into numerical format using one-hot encoding to ensure they can be used in machine learning models.
Splitting Data: Dividing the dataset into features (X) and the target variable (y), then splitting it into training and test sets to evaluate the model's performance on unseen data.
Scaling Data: Normalizing the feature data using standard scaling to ensure all features contribute equally to the model's predictions.
7. Building and Evaluating the Model
A Random Forest Regressor is chosen for predicting app ratings due to its robustness and ability to handle a large number of features. Key steps include:
Model Training: Training the Random Forest model on the training data.
Predictions: Making predictions on the test data to evaluate the model's performance.
Visualization: Creating scatter plots and residual plots to visualize the model's predictions against actual values, which helps in assessing the model's accuracy and identifying any patterns or biases.
Performance Metrics: Evaluating the model using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE). These metrics provide insights into the model's prediction errors.
Accuracy Calculation: Calculating the model's accuracy based on the Mean Absolute Percentage Error (MAPE), which gives a percentage-based evaluation of how close the predictions are to the actual values.
8. Conclusion
The entire process ensures that the data is thoroughly cleaned, explored, and prepared before building a predictive model. Each step is meticulously performed to ensure the reliability and accuracy of the model's predictions. The final model's performance is assessed through various metrics, ensuring it meets the desired accuracy of 90.25% for predicting app ratings in the Google Play Store dataset.
