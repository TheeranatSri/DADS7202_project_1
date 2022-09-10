# DADS7202 Project 1

## Project Hypothesis
We believe that between traditional ML and MLP, MLP will not going to have a better result than traditional ML

## Introduction
This homework is to predict bankruptcy by using binary classification  

## Data
1. Data Source:\
    The data were collected from the Taiwan Economic Journal for the years 1999 to 2009.
    Company bankruptcy was defined based on the business regulations of the Taiwan Stock Exchange 
    (Y = Bankrupt (0/1), X has 95 features). 
2. Data Preparation: 
3. Data Pre-Processing: 
4. Data Splitting:\
    We split data into 2 sets which are Train (56%)/Validate (24%)/Test (20%) 

## Results on Validated data (ML)
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
## Results on Test  data (ML)
![image](https://user-images.githubusercontent.com/88021144/189296152-840d88f7-3313-40fa-8f59-2bbaef06dec7.png)

## Results by (Keras MLP)
 ### ___1.Base model:___
  - Sequentail and parameter of base model
  ![image](https://user-images.githubusercontent.com/33378401/189472700-2c9a6bf0-f2ff-4824-abc7-a48800fb7b30.png)
  - Accuracy on train and validate data set
  ![image](https://user-images.githubusercontent.com/33378401/189472723-d7332e24-e767-450c-8484-6041998d8acc.png)
  - Accuracy on test data set
  ![image](https://user-images.githubusercontent.com/33378401/189472740-6620a154-0089-4f8a-907e-c3295867bbdb.png)
  
 ### ___2.Hyperparameter model by keras tuner:___
  - Tuner parameter
  ![image](https://user-images.githubusercontent.com/33378401/189472748-785212e8-970f-462e-bafb-dbd608f812cf.png)
  - Accuracy on train and validate data set (300 trial and total elapsed time 1 hour 33 minute.!!!)
  ![image](https://user-images.githubusercontent.com/33378401/189472777-e5a61973-c6b6-446d-a659-ceac2a8d480d.png)
  - Sequentail and parameter of the best val_accuracry model
  ![image](https://user-images.githubusercontent.com/33378401/189472785-5aa82952-2c56-431a-9609-62d1a00fe054.png)
  - Accuracy on test data set compare with base model
  ![image](https://user-images.githubusercontent.com/33378401/189472789-d32a2f9c-dbfb-42b6-9b51-54c18fcce439.png)
  - Tensorboard for review hyperparameter of 300 trial
  ![image](https://user-images.githubusercontent.com/33378401/189472793-eaca9780-c300-419e-8d97-f63e351229c1.png)
  
## References
- <https://www.kaggle.com/datasets/fedesoriano/company-bankruptcy-prediction>
- <https://pycaret.org>
- <https://pycaret.readthedocs.io/en/stable/index.html>

## Source
- Deron Liang and Chih-Fong Tsai, deronliang '@' gmail.com; cftsai '@' mgt.ncu.edu.tw, National Central University, Taiwan 
- The data was obtained from UCI Machine Learning Repository:
- <https://archive.ics.uci.edu/ml/datasets/Taiwanese+Bankruptcy+Prediction>

## Relevant Papers 
- Liang, D., Lu, C.-C., Tsai, C.-F., and Shih, G.-A. (2016) Financial Ratios and Corporate Governance Indicators in Bankruptcy Prediction: A Comprehensive Study.
- European Journal of Operational Research, vol. 252, no. 2, pp. 561-572. 
- <https://www.sciencedirect.com/science/article/pii/S0377221716000412>

