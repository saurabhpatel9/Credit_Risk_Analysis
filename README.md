# Credit_Risk_Analysis
## Overview & Purpose
The purpose of this project is to build Machine Learning models to predict credit risk, determining the accuracy based on these models.
In order to evaluate this, the following are the steps involved:

<li>Oversample the data using the RandomOverSampler and SMOTE algorithms.</li>
<li>Undersample the data using the ClusterCentroids algorithm.</li>
<li>Use oversampling and undersampling using the SMOTEENN algorithm.</li>
<li>Compare two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier.</li>

## Results & Analysis 

### RandomOverSampler model
#### 1. Balanced Accuracy Score
    The balanced accuracy score is 64%.
![1-img](https://user-images.githubusercontent.com/86158802/138570966-aa89d1d5-82ee-46cd-8436-a54b694ec921.PNG)

#### 2. Confusion Matrix
    The high_risk precision is about 1% only with 59% sensitivity which makes a F1 of 2% only.
![img2](https://user-images.githubusercontent.com/86158802/138570973-ab9f4aa9-72f4-46f1-a6e0-0742c117bdbe.PNG)

#### 3. Imbalanced Classification Reports
    Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 68%.
![img3](https://user-images.githubusercontent.com/86158802/138570977-a1d7df77-6055-43f2-8b8c-8286ad3810fa.PNG)

### SMOTE model
#### 1. Balanced Accuracy Score
    The balanced accuracy score is 63%, which are quite close to the RandomOverSample Model.
![smote-1](https://user-images.githubusercontent.com/86158802/138571289-c22d79cb-059f-40d6-8725-251db68c1c54.PNG)

#### 2. Confusion Matrix
    The high_risk precision is about 1% only with 64% sensitivity which makes a F1 of 2% only.
![smote-2](https://user-images.githubusercontent.com/86158802/138571298-fa9e13f7-0605-4257-bfb7-cb7847279b63.PNG)

#### 3. Imbalanced Classification Reports
    Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 62%.
![smote-3](https://user-images.githubusercontent.com/86158802/138571304-5ca07cf6-5f6f-4d9e-83f7-d5e54735d6dd.PNG)

### ClusterCentroids model
#### 1. Balanced Accuracy Score
    Here the balanced accuracy score is down to about 51%.
![cc-1](https://user-images.githubusercontent.com/86158802/138571308-fda3dd57-3bb8-4499-858e-cf6f05d92df8.PNG)

#### 2. Confusion Matrix
    The high_risk precision is still 1% only with 59% sensitivity which makes a F1 of 1%.
![cc-2](https://user-images.githubusercontent.com/86158802/138571313-2a8f2305-e399-44a2-9717-b5a2755d815c.PNG)

#### 3. Imbalanced Classification Reports
    Due to the high number of false positives, the low_risk sensitivity is only 44%.
![cc-3](https://user-images.githubusercontent.com/86158802/138571315-206506d7-3769-4277-b9dc-44b4ec48c742.PNG)

### SMOTEENN model	
#### 1. Balanced Accuracy Score
    The balanced accuracy score is about 62%.
![smoteenn-1](https://user-images.githubusercontent.com/86158802/138571332-f073c691-0360-4f7d-87f0-610cbc35e687.PNG)

#### 2. Confusion Matrix
    The high_risk precision is still 1% only with 67% sensitivity which makes a F1 of only 2%.
![smoteenn-2](https://user-images.githubusercontent.com/86158802/138571336-50a2a25e-7909-4feb-85ec-db42a7c8fe35.PNG)

#### 3. Imbalanced Classification Reports
    Due to the high number of false positives, the low_risk sensitivity is 57%.
![smoteenn-3](https://user-images.githubusercontent.com/86158802/138571345-0aade966-5ac2-4850-b09c-537bb839d8d5.PNG)

### BalancedRandomForestClassifier model	
#### 1. Balanced Accuracy Score
    The balanced accuracy score improved to about 79%.
![brf-1](https://user-images.githubusercontent.com/86158802/138571347-130494de-b72f-41df-8a1c-b24affa87a06.PNG)

#### 2. Confusion Matrix
    The high_risk precision is still low at 4% only with 67% sensitivity which makes a F1 of only 7%.
![brf-2](https://user-images.githubusercontent.com/86158802/138571351-b70366e7-eb73-4b47-83ad-de8aa887ec84.PNG)

#### 3. Imbalanced Classification Reports
    Due to a lower number of false positives, the low_risk sensitivity is now 91% with 100% presicion.
![brf-3](https://user-images.githubusercontent.com/86158802/138571353-c0a73aeb-2d86-4198-bd0a-86257deaaad6.PNG)

### EasyEnsembleClassifier model	
#### 1. Balanced Accuracy Score
    Now, the balanced accuracy score is high to about 93%.
![ee-1](https://user-images.githubusercontent.com/86158802/138571364-d26cea02-7d18-4d20-a1db-70d8524ef6fe.PNG)

#### 2. Confusion Matrix
    The high_risk precision is still low at 7% only with 91% sensitivity which makes a F1 of only 14%.
![ee-2](https://user-images.githubusercontent.com/86158802/138571365-4b745384-93fb-4f49-80cb-8c0268aea0f5.PNG)

#### 3. Imbalanced Classification Reports
    Due to a lower number of false positives, the low_risk sensitivity is now 94% with 100% presicion.
![ee-3](https://user-images.githubusercontent.com/86158802/138571366-a119b6ff-3449-4a57-aba1-713113ec4a28.PNG)

## Summary
Every one of the models used to play out the credit risk analysis shows quite less accuracy in deciding whether credit risk is high. 
The Ensemble models brought much greater improvement particularly on the sensibility of the high-risk credits. 
The EasyEnsembleClassifier model shows a review of almost 93% so it identifies practically all high-risk credit. Whereas, with low accuracy, a great deal of low-risk credits are still erroneously recognized as high risk which would be harmful for the bank's credit technique and construe on its income by passing up on those business openings.
Therefore, these machine learning models do not deem fit to evaluate credit risk for the bank.
