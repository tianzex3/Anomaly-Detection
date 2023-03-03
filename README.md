## Case Description:
Banking security systems are designed to protect the assets of their customers by sending alerts to remind customers of seemingly fraud transactions. Sending accurate alerts about the true fraud transaction is meaningful to help banks increase their customers' stickiness by demonstrating the ability to defend customers’ wealth. The primary data source is retrieved from Kaggle, Credit Fraud || Dealing with Imbalanced Datasets. The dataset provides 31 different features and approximately 285k observations. The missing values in the dataset have been cleaned. Due to privacy, most of the features’ names have been scaled and replaced with serial numbers except for transaction and amount. The goal of this project is to develop anomaly detection mechanisms for seemingly credit card fraud transactions that deviate from the normal pattern of transactions. For example, a purchase made in a different country from the cardholder's location may be flagged as suspicious. The mechanisms are expected to not only make the right fraud detection but also reduce false fraud alerts.

![image](https://user-images.githubusercontent.com/90085137/222816791-2878f36d-cdcf-43d5-a4b0-b6179f5d8788.png)

## Methodology
Tool: Over-Sampling, Machine Learning, Deep Learning <br>
File Type: csv <br>
Language: Python <br>

## Available Data Summary
The transaction amount is relatively small. The mean of all the mounts made is approximately USD 88.

There are no "Null" values, so we don't have to work on ways to replace values.

Most of the transactions were Non-Fraud (99.83%) of the time, while Fraud transactions occurs (0.17%) of the time in the dataframe.

## Our project is roughly divided into the following steps:
1. __Data collection and preprocessing__: it involves retrieving a dataset that includes both fraudulent and non-fraudulent transactions, and cleaning the data by removing any errors or remedying inconsistencies.

2. __Feature selection__: it involves selecting a set of influential features that are relevant to the problem of credit card fraud detection using classification methods. Important features can be determined via methods like correlation matrix among different features, dimension reduction techniques such as pca. For example, the location of the merchant, the amount of the transaction, and the time of the transaction are some of the common features that often arise in the problem of credit card fraud detection.

3. __Visualization__: it involves numerous exploratory data analysis that can generate insights to better understand the features and the goals of this project through visual representation of the data, such as distribution of default and non default transactions, abnormal observations, tsne, clustering.

4. __Model training__: Various machine learning models that incorporate different parameters will be trained. The optimal model is expected to distinguish true/false fraud transactions while capturing as many fraud transactions as possible.

5. __Evaluation__: This involves evaluating the performance of the model based on sanity(if fitting properly and data are balanced or not), confusion matrix, and metrics such as accuracy, precision, and recall. The best anomaly-detection model will be selected after comparison.

6. __Business Value/contribution__: After evaluation, if the model performs well, it can be deployed to a live system, where it can flag fraud transactions after required parameters are entered to the system. The baseline of the original system will be evaluated and the effect of this new project will be calculated, which helps to calculate the business value of this project while taking costs of the data analytics teams, project implementation into consideration.

## Reference
https://www.kaggle.com/code/janiobachmann/credit-fraud-dealing-with-imbalanced-datasets/input
