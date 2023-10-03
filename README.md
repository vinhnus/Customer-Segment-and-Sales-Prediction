# Customer-Segment-and-Sales-Prediction

## Situation:
You are working as a Data Analyst in a company that sells cars. The company wants to find ways to marketing for existing customers effectively and new potential customers. Your manager gives you the dataset that includes customers' information in 2019 with their financial attributes along with the sales.

Your tasks:

* Segment the customers based on theirs financial features and provide potential marketing strategies.

* Find new potential customers based on country current financial status, best to find locate individuals who posses one car or less

* Build a simple model to predict the sale amount

Objective:

* Understand the Dataset & cleanup (if required).
* Build a clustering model to cluster data based on their characteristics
* Build Regression models to predict car sales
* Also evaluate the models & compare their respective scores like MAE, MSE, R2, RMSE,.. etc

## DATASETS
This project includes two datasets:
1. The company customers dataset (in 2019)
   
  | Column Name  | Description  |
  |---|---|
  | Customer Name  | Name of customer  |
  | Customer e-mail  | Email of customer  |
  | Country  | Country of customer  |
  | Gender  | Gender of customer 0: Male, 1: Female  |
  | Age  | Customers' age  |
  | Annual Salary  | Customers' salary per year  |
  | Credit Card Debt  | Customers' debt  |
  | Net Worth  | Customers' net worth  |
  | Car Purchase Amount  | Money customers spent on cars |

2. The SCF data - Survey of Consumer Finances (in 2019) by BOARD OF GOVERNORS of the FEDERAL RESERVE SYSTEM. The Survey of Consumer Finances (SCF) is a triennial
   statistical survey of the balance sheet, pension, income and other demographic characteristics of families in the United States; the survey also gathers
   information on the use of financial institutions.
   

## Objectives :
Build clustering models and regression models to segment customers, find potential customers, and forecast company sale revenue

## Project track 
* Data Overview and Data Cleaning

* Exploratory Data Analysis

* Unsupervised Machine Learning Task: Cluster Analysis

* Customer Segmentation Report

* Supervised Machine Learning Task: Build a predictive model to predict company cars' sale amount

## Result

**1. Customer segmentation**

   ![Screenshot 2023-10-03 172705](https://github.com/vinhnus/Customer-Segment-and-Sales-Prediction/assets/132123952/70532548-1ee5-4128-8ee4-2c2c29539ee9)

   KMean determined which cluster each customer's observation belonged to after categorizing the overall population into 6 separate groups. Following that,
   the distribution of the clusters in the general and customer populations may be compared.

   As we can see cluster 1, 2, 3 are underrepresented

   Our customers come mostly from cluster 0 and 5.

   * Cluster 0 represents customer that are in boomer generation and solid financial status, they like honest and clear messaging, clear paths to purchasing, email
     marketing campaigns, customer service, offers and social media. I suggest Traditional advertising; loyalty programs; word of mouth, email and social
     marketing; and incentives. 
   * Cluster 5 represents middle income millennials, we could try influencer marketing, reviews, videos, TikTok, Instagram, Snapchat, YouTube,
     mobile interactions, and social selling and advertising.Testimonial and influencer
     marketing, short videos, social and economic causes, and apps on smartphones.
     
   * **Potential customer** If the company want to target potential customers based on country current financial status, from what the model segment, they mainly
     come from cluster 0, 5 also. I suggest **a pay-in-installments, or having special offers for first-time buyers,...**

   **CALL TO ACTION**

   The base core customer represents a smaller portion of the population when it comes to the income, age, or social classes analysis, even though there is a clear
   profile indicating specific segments of the population that are more likely to become customers of the company.

   It could also be seen as a great opportunity for the company to promote different marketing strategies, launched different and more affordable of the current
   products that could be,
   for example, purchased by people with lower incomes.

   At the same time, it’s possible to reach out to younger people that are especially concerned about environmentalism issues, investing in directed marketing
   campaigns that speak with these new generations. They could potentially become customers for a lifetime.

**2. Predictive Modeling**

   I use the company dataset to train and test purposes. My predict variable is the " Car Purchase Amount", and input variable will be the customers' financial
   attributes.

   The models I used for training and testing are :

   * Linear Regression
  
   * SVM
  
   * KNR
  
   * Decision Tree
  
   * Random Forest
  
   After traning and evaluating, I decided to use three models **Random Forest**, **Decision Tree**, **KNR** for hyperparameter tuning

   ![Screenshot 2023-10-03 181513](https://github.com/vinhnus/Customer-Segment-and-Sales-Prediction/assets/132123952/6964b795-c55e-46c2-813e-16f19abbf1d9)

   **Random Forest** is the best model for this prediction since it has better MAE compared to the other two models.

   This plot shows how well the Random Forest predict the sales amount compared to the actual values. 

   ![Screenshot 2023-10-03 182150](https://github.com/vinhnus/Customer-Segment-and-Sales-Prediction/assets/132123952/bc099c43-2588-4357-9bd5-e543dc2a48e7)

## Improvements
**Clustering** We could try different clustering algorithms like DBSCAN, Hierarchical clustering, etc for better results

**Predicting** Use different scaling methods, wide range of hyperparameter tuning, GridSearchCV for exhaustive search

