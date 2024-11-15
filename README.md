# Loan Prediction Project

## Overview
This project aims to predict loan eligibility for applicants based on various features. Using machine learning algorithms, the model learns from historical data to determine if an applicant qualifies for a loan. The dataset includes factors such as applicant income, loan amount, credit history, and more.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Dataset

The dataset contains the following key features:

| Column Name        | Description                                                     |
|--------------------|-----------------------------------------------------------------|
| `Loan_ID`          | Unique identifier for each loan application                     |
| `Gender`           | Gender of the applicant                                         |
| `Married`          | Marital status (Yes/No)                                         |
| `Dependents`       | Number of dependents                                            |
| `Education`        | Education level of the applicant (Graduate/Not Graduate)        |
| `Self_Employed`    | Whether the applicant is self-employed (Yes/No)                 |
| `ApplicantIncome`  | Income of the applicant (numeric)                               |
| `CoapplicantIncome`| Income of the co-applicant (numeric)                            |
| `LoanAmount`       | Requested loan amount (numeric)                                 |
| `Loan_Amount_Term` | Duration of the loan in months                                  |
| `Credit_History`   | Credit history of the applicant (1: Good, 0: Bad)               |
| `Property_Area`    | Type of area (Urban/Rural/Semiurban)                            |
| `Loan_Status`      | Target variable (Y: Loan approved, N: Loan not approved)        |


## Project Structure

The project repository contains the following files:

- `train_data.csv`: Training dataset used for building the model.
- `loan_prediction.ipynb`: Jupyter notebook where data analysis, preprocessing, and model training are performed.
- `requirements.txt`: List of libraries and dependencies needed to run the project.
- `README.md`: Project documentation.
## Installation

To run the project locally, you can follow these steps:

1. Clone the repository:

   ```bash
   git clone [https://github.com/naoufal2807/Loan_prediction_project.git
2. Navigate to the project directory:

   ```bash
   cd Loan_prediction_project

3. Create a virtual environment and install the required dependencies:

   ```bash
   python3 -m venv env
   source env/bin/activate
   pip install -r requirements.txt
4. Open the Jupyter notebook to run the model:
   ```bash
   jupyter notebook loan_prediction.ipynb

## Models Used :
The following machine learning algorithms were explored in this project:

- `Logistic Regression`: A baseline model for binary classification.
- `Random Forest Classifier`: A more complex model with better performance on non-linear data.
- `Gradient Boosting`: A powerful boosting method that combines multiple weak learners for improved accuracy.
## Key Steps
1. Data Preprocessing:

- Handle missing values.
- Convert categorical variables into numerical representations.
- Normalize or scale continuous features where necessary.
2. Model Training:

- Split the dataset into training, validation  and testing sets.
- Train the models using different algorithms.
- Evaluate model performance using accuracy, precision, recall, and F1 score.
3. Model Evaluation:

- Compare different models to choose the best performing one based on evaluation metrics.
- Use Stratified K-Fold cross-validation to assess model generalization.

## Results
The model achieved an accuracy of 87% on the test set. The Random Forest classifier performed the best among the models, followed by Gradient Boosting.

## Future Improvements 
Hyperparameter tuning to further optimize model performance.
Explore more advanced models such as XGBoost or CatBoost.
Incorporate feature engineering to better capture the relationship between features and the target variable.
Deploy the model using Flask or Django for real-time loan predictions.

## Contributing
If you’d like to contribute to this project, feel free to fork the repository and submit a pull request. Any suggestions for improvements are welcome!



