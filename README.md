# Ecommerce_Churn_Analysis

source: https://www.kaggle.com/datasets/ankitverma2010/ecommerce-customer-churn-analysis-and-prediction?resource=download

An ecommerce platform hired a team of data scientist to reduce churn customers rate. We analyzed the data to provide recommendations for improvements and used machine learning to identify which customers are going to churn. 

Data preparation includes dropping unnecessassary columns, dropping duplicates, and standardizing text.

In exploratory data analysis, through Mann-Whitney test, we found out that exist significant difference between churn and loyal customers in tenure length, city tier, warehouse distance, number of device registered, satisfaction score, complaints, days since last order and cashback amount. This means customers received different treatment that led to loyal or churn customers on these factors. When analyzing customers information using Chi-Square, we found out that Gender, Marital Status, Login Device, Payment Mode, and Order Category exist significant difference. Which means our services are not uniformed across all sectors.

When implementing machine learning, we cleaned the data by imputing missing values, scaling for numerical data and encoding for categorical data. We used 7 models in cross validation and tuned top 2 models for best performance. K-NN and XGboost turned out to be 2 best models and after 1st tuning, K-NN still performs the best. Hence, we tune K-NN once more and resulted in 98% recall. Identified churn customers will be prioritized to receive treatment such as notification, promo and reminder etc. 

Before ML, 167 customers would churn and total loss would be $ 6,680. After ML, 6 customers would churn that would lead to $ 240 loss.

However, this ML is not without limitation. we recommend to monitor performance regularly, add more data, regular testing and validation, and consult with domain expert or crossfunction team.
