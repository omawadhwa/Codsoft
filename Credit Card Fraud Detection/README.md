# Credit Card Fraud Detection

## Project Overview

This project focuses on building a machine learning model for detecting fraudulent credit card transactions. With the rise in online transactions, fraud detection has become an essential part of maintaining user trust and financial security. This project utilizes a comprehensive dataset containing features from genuine and fraudulent transactions to train the model.

## Data Description

The dataset comprises transactions made by credit cards, where each transaction is labeled as fraudulent or genuine. It includes 31 features: 28 anonymized features (V1 to V28), the transaction amount, the transaction time, and the class indicating fraud (1) or not (0). The anonymized features result from a PCA transformation due to confidentiality issues.

## Data Preprocessing

Initial data exploration revealed no missing values within the dataset, ensuring a solid foundation for model training. However, the dataset contained 1081 duplicate transactions, which were subsequently removed to prevent bias in the model. The dataset exhibited a significant class imbalance, with fraudulent transactions being much less common than genuine ones, necessitating careful handling to avoid model bias towards the majority class.

## Exploratory Data Analysis (EDA)

The exploratory analysis included visualizing distributions, correlations, and relationships between features. This phase was critical for understanding the data's structure and the underlying patterns distinguishing fraudulent transactions from genuine ones.

## Handling Class Imbalance

The stark imbalance between the classes was addressed using the Synthetic Minority Over-sampling Technique (SMOTE), which artificially generates new minority class samples, balancing the dataset without losing crucial information. This approach significantly improved the model's ability to detect fraudulent transactions.

## Feature Engineering and Data Normalization

Feature engineering involved creating new features that could potentially improve the model's performance. Data normalization ensured that all features contributed equally to the model training process, preventing features with larger scales from dominating the model's decision-making process.

## Model Development and Evaluation

Several machine learning models were trained and evaluated, including Logistic Regression and Random Forest Classifier. The models were assessed based on precision, recall, F1-score, and the ROC AUC score to ensure a comprehensive evaluation of their performance in classifying transactions accurately.

## Results

The final models demonstrated a high ability to distinguish between fraudulent and genuine transactions, with the Random Forest Classifier showing particularly promising results. The application of SMOTE for handling class imbalance proved to be effective, as evidenced by the improvement in model performance metrics.

## Conclusion

This project highlights the importance of thorough data preprocessing, exploratory data analysis, and appropriate handling of class imbalance in building effective fraud detection systems. The machine learning models developed through this project can significantly contribute to identifying fraudulent transactions, thereby enhancing the security of credit card transactions.