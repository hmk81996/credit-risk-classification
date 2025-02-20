# credit-risk-classification
Supervised Machine Learning - Data Analytics Course Module 20

# Task
Train and evaluate a model based on loan risk using a dataset of historical lending activity from a peer-to-peer lending services company. Build a model that can identify the creditworthiness of borrowers.

# Methodology
1. Split the data into **training and testing** sets.
2. Create a **logistic regression model** with the original data.
3. Evaluate the model's performance:
   - Generate a confusion matrix.
   - Generate a classification report.
4. Write a Credit Risk Analysis report.

# Credit Risk Analysis Report
## Overview
The purpose of this analysis is to build a model that allows a peer-to-peer lending services company to identify the creditworthiness of borrowers. The model will train and test historical lending activity from the company, ultimately allowing it to label a potential loan as "healthy" or "high-risk". 

## Results

### Visualization of Model's Performance
#### Confusion Matrix Heat Map

![Heat Map](Images/heatmap.png)

**The confusion matrix shows 110 false positives.** These were incorrectly predicted positive cases; that is, they were labeled "high-risk" but are actually "healthy". **The matrix shows 36 false negatives.** These were labled "healthy" but are actually "high-risk". 
- The *accuracy* score of this classification model is .99 which means that overall, it is performing very well.

- The logistic regression model predicts _healthy loans_ with *perfect precision* (1.00) and predicts _high-risk loans_ less with *less precision* (.84). 

- The *recall* for healthy loans is .99 and for high risk loans it is .94. Overall, the recall is high which means it is performing well when identifying true positives but some high-risk loans are being missed. This error could lead to increased financial risk for lenders.

- The *f1-score* is at 1.00 for healthy loans, meaning recall and precision were high. However, the f1-score is .89 for high-risk loans. While recall was strong for high-risk loans, it's precision was low. This lets us know that while overall accuracy is high, we need to continue refining the model to better predict high-risk loans. 

## Summary

Overall, this machine learning model appears to yield highly accurate results. However, a closer look shows that it requires further optimization. While it does well prediciting creditworthiness for healthy loan potential, it does less well in predicting high-risk loan cases. The consequences of mislabeling "healthy loans" as "high-risk" might be that individuals or businesses miss out on crucial funding or at best, undergo unnessary review. Likewise, mislabeling a "high-risk loan" as a "healthy loan" could increase financial risk to a lender. Given these potential errors and the weight of their impact, the model needs to be fine-tuned to produce higher scores for precision, recall and f-1 values before deployment by the lending services company.


 




