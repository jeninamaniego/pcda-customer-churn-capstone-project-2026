# Predicting Customer Churn – Capstone Project 2026

## Project Overview

This capstone project explores how machine learning can be used to predict customer churn and support data-driven retention strategies.

Customer churn is a key business problem because losing customers can reduce revenue, weaken customer relationships, and increase acquisition costs. The aim of this project is not only to predict which customers are likely to churn, but also to understand the factors driving churn and identify which customers should be prioritised for retention activity.

## Business Objective

The project aims to answer the following question:

**Can machine learning help identify customers at risk of churn and support more targeted retention strategies?**

The analysis focuses on:

- Predicting whether a customer will churn
- Identifying key churn drivers
- Segmenting customers using clustering
- Prioritising high-risk, high-value customers for retention

## Dataset

The project uses an ecommerce customer churn dataset containing customer demographic, behavioural, engagement, and transactional features.

The dataset includes:

- 50,000 customer records
- 25+ features
- Behavioural data such as cart abandonment rate, session duration, and login frequency
- Customer value data such as lifetime value and purchase activity
- Target variable: `Churned`

The target variable indicates whether a customer was retained or churned.

## Methods Used

The analysis was completed in Python using a Jupyter Notebook.

Main techniques used:

- Data cleaning and preprocessing
- One-hot encoding for categorical variables
- Train-test split
- Dummy Classifier as a baseline model
- Decision Tree Classifier
- Decision Tree tuning using maximum depth
- Confusion matrix and classification report
- Random Forest Classifier
- Feature importance analysis
- K-Means clustering
- Customer prioritisation using churn probability and lifetime value

## Modelling Approach

A Dummy Classifier was first used as a baseline model. This helped establish a benchmark by predicting the majority class.

A Decision Tree model was then used as the first predictive model because it is interpretable and helps identify important churn drivers. The model was improved by tuning tree depth to reduce overfitting and improve generalisation.

A Random Forest model was then developed to improve prediction performance and reduce overfitting. This model was selected as the preferred model because it provided better generalisation and stronger performance in identifying churned customers.

## Key Findings

The analysis identified several important churn drivers:

- Customer lifetime value
- Customer service calls
- Cart abandonment rate
- Discount usage
- Days since last purchase
- Email open rate

Cart abandonment rate was also tested separately by removing it from the model. The decrease in model performance confirmed that it is an important predictor, but not the only factor influencing churn.

## Clustering and Optimisation

K-Means clustering was used to segment customers into different behavioural groups. This helped identify customer profiles such as high-value customers, low-engagement customers, and higher-risk churn groups.

An optimisation approach was then applied by combining churn probability with customer lifetime value. This allowed customers to be ranked by priority, helping identify which high-risk, high-value customers should be targeted first for retention activity.

## Business Recommendations

Based on the analysis, businesses should:

1. Prioritise high-risk, high-value customers for retention campaigns.
2. Reduce cart abandonment through reminders, improved user experience, or targeted incentives.
3. Improve customer service interactions, as service-related issues appear to be linked with churn risk.
4. Use customer segmentation to tailor retention strategies to different customer groups.

## Conclusion

This project demonstrates how machine learning can support customer retention by predicting churn, identifying key drivers, and helping businesses prioritise action.

The Random Forest model provided the strongest overall approach, while clustering and optimisation extended the analysis from prediction to practical decision-making.

## Repository Contents

- `Predicting Customer Churn - Capstone Project 2026 (JM) (FINAL).ipynb` – full Jupyter Notebook containing the analysis and modelling workflow
- Dataset file – ecommerce customer churn dataset, if included in repository
- README.md – project summary and documentation

## Tools and Libraries

- Python
- pandas
- NumPy
- matplotlib
- seaborn
- scikit-learn
- Jupyter Notebook

## Author

Jenina Maniego  
Professional Certificate in Data Analytics Capstone Project 2026
