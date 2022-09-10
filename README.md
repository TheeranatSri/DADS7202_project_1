# DADS7202 Project 1

# Project Hypothesis
We believe that between Traditional Machine Learning and MLP (Multilayer Perceptions), Traditional ML will have a better result than MLP. 

# Introduction
This project aims to predict bankruptcy by comparing results between various traditional machine learning models and MLP using Keras to perform binary classification. 

# Data
1. Data Source:\
    The data were collected from the Taiwan Economic Journal for the years 1999 to 2009.
    Company bankruptcy was defined based on the business regulations of the Taiwan Stock Exchange 
    (Y = Bankrupt (0/1), X has 95 features). 
2. Data Preparation: 
3. Data Pre-Processing: 

4. Data Splitting:\
    We split data into 2 sets which are Train (56%)/Validate (24%)/Test (20%) 
## ML Model
## Results on Validated data
 ### ___1.  Accuracy table___
![image](https://user-images.githubusercontent.com/88021144/189294004-9ff55d08-5745-4f91-922d-8e236777ab82.png)
 ### ___2.  Mean and Standard deviation for 10 Fold___
 ![image](https://user-images.githubusercontent.com/88021144/189295088-9d3e053a-22cf-486a-9036-27d1635dff8a.png)
 ### ___3.  AUC-ROC Curves___
 ![image](https://user-images.githubusercontent.com/88021144/189295134-132476c8-a55d-4dac-b3cc-83011339ce4c.png)
 ### ___4.  Confusion Matrix___
 ![image](https://user-images.githubusercontent.com/88021144/189295159-ad7a5709-41c0-426b-97cf-7860db97ec5c.png)
 ### ___5.  Precision-Recall Curve___
 ![image](https://user-images.githubusercontent.com/88021144/189295211-9d55a3ad-8d00-4a76-ba65-7b0551a074f9.png)
 ### ___6.  Prediction Error___
 ![image](https://user-images.githubusercontent.com/88021144/189295243-33696410-882c-4bf2-b99e-0bdd9fdf9748.png)
 ### ___7.  Class Report___
 ![image](https://user-images.githubusercontent.com/88021144/189295264-676e80eb-ef4d-410d-a8ee-2a1b2b9c3473.png)
### ___8.  Feature Importance___
![image](https://user-images.githubusercontent.com/88021144/189295289-a97d55eb-c1c3-4c78-953d-1f55e1e3e45c.png)
## Results on Test  data
![image](https://user-images.githubusercontent.com/88021144/189296152-840d88f7-3313-40fa-8f59-2bbaef06dec7.png)
# MLP ModelResults by (Keras MLP)
 ### ___1.Basic model (Model in class):___
  - Sequentail and parameter of model
  
  ![image](https://user-images.githubusercontent.com/33378401/189479365-c8c48931-b67a-49a7-a620-22ab6980f7ac.png)
  
  - Accuracy on train and validate data set
  
  ![image](https://user-images.githubusercontent.com/33378401/189479373-df333a86-ec6b-47db-b5be-67c16a4eaf51.png)
  
  - Accuracy on test data set = 0.8872
  
 ### ___2.Hyperparameter model by keras tuner:___
  - Sequentail and parameter of model
  
  ![image](https://user-images.githubusercontent.com/33378401/189472748-785212e8-970f-462e-bafb-dbd608f812cf.png)
  
  - Accuracy on train and validate data set (300 trial and total elapsed time 1 hour 33 minute.!!!)
  
  ![image](https://user-images.githubusercontent.com/33378401/189472777-e5a61973-c6b6-446d-a659-ceac2a8d480d.png)
  
  - Sequentail and parameter of the best val_accuracry model
  
  ![image](https://user-images.githubusercontent.com/33378401/189472785-5aa82952-2c56-431a-9609-62d1a00fe054.png)
  
  - Accuracy on test data set = 0.9560
  
  - Tensorboard for review hyperparameter of 300 trial
  
  ![image](https://user-images.githubusercontent.com/33378401/189472793-eaca9780-c300-419e-8d97-f63e351229c1.png)
  
 ### ___3.Manual hyperparameter model:___
  - Sequentail and parameter of model
  
 ![image](https://user-images.githubusercontent.com/33378401/189479752-4fc352d0-04cc-44d2-8626-cb96a7eda86d.png)
 
 - Accuracy on train and validate data set
 
 ![image](https://user-images.githubusercontent.com/33378401/189479794-337b9737-ecf0-4edd-ab08-1a7c269bf31d.png)
 
 - Accuracy on test data set = 0.9651

 ## ___Summary of MLP___
 ![image](https://user-images.githubusercontent.com/33378401/189479945-10f21630-4881-4c5a-9b50-276d80e06e7a.png)
 
# Summary
The results showed that the traditional model
It provides better accuracy compared to Multilayer Perceptions Basic Model, Hyperparameter Tuner by Keras Tuner, and Manual Hyperparameter Model at 8.06%, 1.51% and 1.90%, respectively, which is why Manual Hyperparameter Model is more accurate. Hyperparameter Tuner by Keras Tuner comes in part by adding layers to the model.
# References
- <https://www.kaggle.com/datasets/fedesoriano/company-bankruptcy-prediction>
- <https://pycaret.org>
- <https://pycaret.readthedocs.io/en/stable/index.html>

# Source
- Deron Liang and Chih-Fong Tsai, deronliang '@' gmail.com; cftsai '@' mgt.ncu.edu.tw, National Central University, Taiwan 
- The data was obtained from UCI Machine Learning Repository:
- <https://archive.ics.uci.edu/ml/datasets/Taiwanese+Bankruptcy+Prediction>

# Relevant Papers 
- Liang, D., Lu, C.-C., Tsai, C.-F., and Shih, G.-A. (2016) Financial Ratios and Corporate Governance Indicators in Bankruptcy Prediction: A Comprehensive Study.
- European Journal of Operational Research, vol. 252, no. 2, pp. 561-572. 
- <https://www.sciencedirect.com/science/article/pii/S0377221716000412>

