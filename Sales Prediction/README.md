# Sales Prediction

## Project Overview
This project focuses on predicting sales based on advertising budgets across multiple channels, including TV, Radio, and Newspaper. Utilizing a dataset containing historical advertising spend and corresponding sales figures, the goal was to develop a machine learning model capable of accurately forecasting sales from future advertising investments. This project involved data preparation, exploratory data analysis (EDA), feature selection, model training and evaluation, hyperparameter tuning, and final model selection.

## Data Preparation and Cleaning
The dataset was meticulously cleaned and prepared for analysis. This process involved checking for and handling missing values, duplicates, and outliers, ensuring the data was in an optimal state for modeling.

## Exploratory Data Analysis (EDA)
Comprehensive EDA was conducted to understand the relationships between advertising budgets and sales. Visualizations such as histograms, scatter plots, and correlation matrices provided insights into how each advertising channel impacts sales. This phase was crucial for identifying significant predictors and informing the feature selection process.

## Feature Selection
Based on EDA findings, it was determined that the TV advertising budget had the most substantial impact on sales, followed by Radio and Newspaper. This understanding guided the selection of features for the predictive models, with a focus on those most correlated with sales outcomes.

## Model Training and Evaluation
Multiple regression models were explored to predict sales, including:
- Linear Regression
- Ridge Regression
- Lasso Regression
- Decision Tree Regressor
- Random Forest Regressor
- XGBoost

Each model was evaluated using the Root Mean Squared Error (RMSE) metric to assess predictive accuracy. This process identified the Random Forest and XGBoost models as top performers.

## Hyperparameter Tuning
Hyperparameter tuning was performed on the Random Forest model to optimize its parameters, utilizing techniques such as GridSearchCV. This process led to the identification of an optimal set of parameters that minimized the RMSE, enhancing the model's predictive accuracy.

## Final Model Evaluation
The Random Forest model, with its tuned hyperparameters, was re-trained on the entire training dataset and evaluated on a separate test set. This final evaluation confirmed the model's high predictive accuracy and generalization capability to unseen data.

## Visualization and Interpretation
To gain insights into the decision-making process of the model, one of the decision trees from the Random Forest ensemble was visualized. This visualization helped interpret how different features influenced sales predictions, providing valuable business insights into advertising budget allocation.

## Conclusion
The project successfully developed a predictive model that can accurately forecast sales based on advertising budgets. The Random Forest and XGBoost models, with their respective tunings, emerged as the most effective, offering precise sales predictions that can guide strategic advertising decisions. This project showcased the application of machine learning techniques in solving a real-world business problem, demonstrating the potential of data-driven decision-making in optimizing advertising strategies.