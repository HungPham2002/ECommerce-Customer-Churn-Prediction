<p align="center" dir="auto">
  <a href="https://www.uit.edu.vn/" title="Trường Đại học Công nghệ Thông tin" rel="nofollow">
    <img src="https://camo.githubusercontent.com/29fa0dade8ce1281054a2a4844513e68f8868f15057452c709392fe49b01d398/68747470733a2f2f692e696d6775722e636f6d2f576d4d6e5352742e706e67" alt="Trường Đại học Công nghệ Thông tin | University of Information Technology" data-canonical-src="https://i.imgur.com/WmMnSRt.png" style="max-width: 100%;">
  </a>
</p>
<h1 align="center" tabindex="-1" dir="auto"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><b>IS334.N21.TMCL - ECOMMERCE</b></h1>
  
# Customer Churn Prediction
- Class: ECOMMERCE - IS334.N21.TMCL
- Lecturer: Mr. Do Duy Thanh
## Introduction 
- This is my Ecommerce project, I build to only research and learn about Machine Learning.
- Deep learning model notebook as extra (Deep neural is a complicated process. in reality, simple things is usually more effective), I have not understood it yet. I'm not sure it work correctly and effectively. Maybe it overfit and I do not see that :DD So I do not recommend to consult this one.
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
- Feature Featuring: The problem requires us to have the knowledge of an expert in the field we are solving. We need to understand the features of the data, which features will affect the desired output
- Model selection: there are many methods to solve this problem, Logistic Regression, K algorithms, classification algorithms, neural networks,...
## Procession:
Details of data preprocessing, training and evaluation of the model, I made a note in the notebook, please read it.
## Note
+ those Lib without in colab just are used for visualizing data and visualizing evaluation or Interact between features. If only training model you can ignore that step because it install and we restart time and rerun -> wasting time :V
+ In Ecommerce project, We requied to create a dashboard to visualize data. this is the URL to Dashboard project: https://github.com/HungPham2002/Dashboard_ECommerce
## References:
### [1] Susan Li: Predict Customer Churn – Logistic Regression, Decision Tree and Random Forest (2017).
### [2] Lalwani, P., Mishra, M. K., Chadha, J. S. and Sethi, P., “Customer churn prediction system: A machine learning approach”, 2022.
### [3] Asthana P: A comparison of machine learning techniques for customer churn prediction. International Journal of Pure and Applied Mathematics (2018).
### [4] Hyperparameters and Tuning Strategies for Random Forest by Philipp Probst, Marvin Wright and Anne-Laure Boulesteix (February 27, 2019)
### [5] Qureshi, S.A., Rehman, A.S., Qamar, A.M., Kamal, A., Rehman, A.: Telecommunication subscribers’ churn prediction model using machine learning. In: Eighth International Conference on Digital Information Management (ICDIM 2013)
### [6] https://www.analyticsvidhya.com/blog/2020/03/beginners-guide-random-forest-hyperparameter-tuning/
### [7] Umayaparvathi V, Iyakutti K: A survey on customer churn prediction in the telecom industry: Datasets, methods and metrics. International Research Journal of Engineering and Technology (IRJET) (2016).
### [8] https://plainenglish.io/blog/decision-tree-parameters-explanations-tuning-a2b0749976e5
### [9] Altexsoft: Customer Churn Prediction Using Machine Learning: Main Approaches and Models
### [10] https://stackoverflow.com/questions/36107820/how-to-tune-parameters-in-random-forest-using-scikit-learn
### [11] Zakria Saad, Customer churn prediction on Telecom dataset
### [12] Germann, F, Lilien, G.L, Fiedler, L, and Kraus, M., “Do retailers benefit from deploying customer analytics?”, Journal of Retailing (2014).
### [13] Mishra, A. and Reddy, U. S., “A novel approach for churn prediction using deep learning”, Proceedings of the IEEE International Conference on Computational Intelligence and Computing Research (ICCIC), Coimbatore India, 1–4, (2017).
### [14] Using Decision Trees to Predict Customer Churn (Published On: 10 April 2020 - By Cybiant)

