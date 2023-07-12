# Hello, 
- This is my Ecommerce project, I build to only research and learn about Machine Learning.
- Deep learning model notebook as extra (Deep neural is a complicated process. in reality, simple things is usually more effective), I have not understood it yet. I'm not sure it work correctly and effectively. Maybe it overfit and I do not see that :DD So I do not recommend to consult this one.
# Customer Churn Prediction 
## Context
In today's highly competitive business landscape, retaining customers is crucial for the success of an organization. A customer churn prediction model using various machine learning algorithms including logistic regression, random forest, Decision Tree
## Dataset: 
  - Content
Each row represents a customer, each column contains customer’s attributes described on the column Metadata.

  - The data set includes information about:
    + Customers who left within the last month – the column is called Churn
    + Services that each customer has signed up for – phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies
    + Customer account information – how long they’ve been a customer, contract, payment method, paperless billing, monthly charges, and total charges
    + Demographic info about customers – gender, age range, and if they have partners and dependents
  - Source: https://www.kaggle.com/datasets/blastchar/telco-customer-churn
## Pipeline:
![pipeline](https://drive.google.com/uc?export=view&id=1PM7_tyPj0Jovt3QpaPhnbbPiHM1KZV2G)
## Difficult Points:
![different points](https://drive.google.com/uc?export=view&id=14K4atm5829Lb3UhKss_STpQ1sk8tUihI)
- Imbalanced data: In fact, the data we collect will often not have a balance between classes (stayed/churned/...). This is understandable because if the 'churn' is balanced with the 'stayed' class, the organization is on the verge of bankruptcy. The harm of data imbalance is very serious. 
  + Eg: Suppose we have 100 samples, 99 class 'non churn' and 1 class 'churn'. The model only needs to make predictions that are all 'non churn' to be 99% accurate, perfect. But in reality it is really useless.
  + To solve this problem, We have many methods to solve. The simplest is that we will change the evaluation metrics, specifically we will no longer use the 'accuracy' metrics.
- Feature Featuring: The problem requires us to have the knowledge of an expert in the field we are solving. We need to understand the characteristics of the data, which characteristics will affect the desired outcome
- Model selection: there are many methods to solve this problem, Logistic Regression, K algorithms, classification algorithms, neural networks,...
## Procession:
Details of data preprocessing, training and evaluation of the model, I made a note in the notebook, please read it.
## Note
+ those Lib without in colab just are used for visualizing data and visualizing evaluation or Interact between features. If only training model you can ignore that step because it install and we restart time and rerun -> wasting time :V
+ In Ecommerce project, We requied to create a dashboard to visualize data. this is the URL to Dashboard project: https://github.com/HungPham2002/Dashboard_ECommerce
