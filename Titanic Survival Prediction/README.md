# Titanic Survival Prediction

## Project Overview
This project focuses on predicting the survival of passengers aboard the Titanic, leveraging machine learning techniques. The dataset used contains various features of the passengers, including age, sex, passenger class, and fare, among others. Through exploratory data analysis, data preprocessing, and model building, this project aims to accurately predict survival outcomes.

## Data Description
The dataset includes the following key features:
- **PassengerId**: An identifier for each passenger.
- **Survived**: Survival (0 = No, 1 = Yes).
- **Pclass**: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd).
- **Name**: Passenger's name.
- **Sex**: Passenger's sex.
- **Age**: Passenger's age in years.
- **SibSp**: Number of siblings/spouses aboard.
- **Parch**: Number of parents/children aboard.
- **Ticket**: Ticket number.
- **Fare**: Passenger fare.
- **Cabin**: Cabin number.
- **Embarked**: Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).

## Methodology
### Exploratory Data Analysis (EDA)
- Conducted comprehensive EDA to understand data distributions, missing values, and potential correlations between features.
- Visualized data distributions and relationships using histograms, box plots, and scatter plots.

### Data Preprocessing
- Handled missing values in `Age`, `Cabin`, and `Embarked` features through imputation.
- Encoded categorical variables like `Sex` and `Embarked` using one-hot encoding.
- Normalized continuous variables such as `Age` and `Fare`.

### Model Building and Evaluation
- **Logistic Regression**: Served as the baseline model, providing initial insights into the dataset's predictability.
- **Decision Tree Classifier**: Explored to capture non-linear relationships between features.
- **Random Forest Classifier**: Utilized to improve prediction accuracy through ensemble learning. Hyperparameter tuning was performed to optimize the model.

### Hyperparameter Tuning
- Conducted hyperparameter tuning on the Random Forest model using GridSearchCV to find the optimal model configuration.

### Model Evaluation
- Evaluated models based on accuracy and further analyzed performance using confusion matrices to understand true positives, false positives, true negatives, and false negatives.

## Key Findings
- The Random Forest Classifier, with tuned hyperparameters, provided the best prediction accuracy among the models tested.
- Feature importance analysis revealed that variables like `Sex`, `Pclass`, and `Age` were significant predictors of survival.

## Conclusion
The project successfully demonstrates the application of machine learning techniques to predict the survival of Titanic passengers. Through iterative exploration, preprocessing, and model optimization, the project highlights the power of ensemble methods like Random Forest in handling classification tasks.