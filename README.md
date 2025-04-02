# Bank-Churn-Prediction
## Project Overview
In this project, we aim to predict customer churn from a dataset containing features such as customer credit score, geography, gender, age, tenure, and other banking-related information. The goal is to apply different machine learning models to this dataset and evaluate their performance in predicting churn.

## Dataset
The dataset used in this project is the Churn_Modelling.csv dataset, which contains 10,000 customer records with the following columns:

- RowNumber: Row number of the record.

- CustomerId: Unique ID for the customer.

- Surname: Surname of the customer.

- CreditScore: Customer's credit score.

- Geography: The country where the customer resides (France, Spain, Germany).

- Gender: Gender of the customer (Male, Female).

- Age: Age of the customer.

- Tenure: The number of years the customer has been with the bank.

- Balance: Account balance of the customer.

- NumOfProducts: Number of products the customer has with the bank.

- HasCrCard: Whether the customer has a credit card (1 = Yes, 0 = No).

- IsActiveMember: Whether the customer is an active member (1 = Yes, 0 = No).

- EstimatedSalary: Estimated annual salary of the customer.

- Exited: Target variable representing whether the customer exited (1) or stayed (0).

## Steps Involved
### 1. Data Preprocessing
- Loading the Dataset: The dataset is loaded and examined for the first few rows.

- Handling Missing Values: Checked for null values, and none were found.

- Feature Selection: Irrelevant features (such as RowNumber, CustomerId, and Surname) were removed.

- Encoding Categorical Data: Categorical features like Geography and Gender were encoded into numerical variables.

### 2. Addressing Class Imbalance
SMOTE (Synthetic Minority Oversampling Technique) was used to balance the target variable (Exited), as the dataset was imbalanced (more customers who stayed than exited).

### 3. Model Training & Evaluation
Different machine learning models were applied to the dataset, including:

- Logistic Regression (LR)

- Support Vector Classifier (SVC)

- K-Nearest Neighbors (KNN)

- Decision Tree Classifier (DT)

- Random Forest Classifier (RF)

- Gradient Boosting Classifier (GBC)

Each model was evaluated using accuracy.
### 4. Feature Scaling
Standard scaling was applied to the features to bring them to the same scale, improving the performance of the models.

### 5. Saving model
Model was saved as pickle file
## Results
The best performing model was Random Forest Classifier, achieving an accuracy of approximately 87% on the test data. indicating that the model performs well in predicting customer churn.
