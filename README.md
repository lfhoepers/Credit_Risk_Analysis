# Module 17 Challenge

## Overview of the Credit Risk Analysis

This project's main objective is to build and evaluate several machine learning models to predict credit risk. We used the following procedures:

- Oversample the data using the RandomOverSampler and SMOTE algorithms.
- Undersample the data using the ClusterCentroids algorithm.
- Use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm.
- Compare two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier.

Follow the 2 codes.

[Credit_Risk_Resampling.ipynb](https://github.com/lfhoepers/Credit_Risk_Analysis/blob/1aa205b4ed59a9ad7435440e1144ece5254c8758/credit_risk_resampling.ipynb)

[Credit_Risk_Ensemble.ipynb](https://github.com/lfhoepers/Credit_Risk_Analysis/blob/0857c136765224e4eb0c4b2802b6f7de5b9b8c1a/credit_risk_ensemble.ipynb)



## Results:


- RandomOverSampler model

![image](https://user-images.githubusercontent.com/100812079/176059222-7aee9c54-49d6-441a-9c8e-a69fccb0d5c7.png)

The balanced accuracy score is 65%.
The high_risk precision is about 1% only with 62% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is  100% with a sensitivity of 68%.


- SMOTE model

![image](https://user-images.githubusercontent.com/100812079/176059489-83a2ff03-ccf3-4ff0-9a19-9b546fadaadb.png)

The balanced accuracy score is 64%.
The high_risk precision is about 1% only with 63% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is 100% with a sensitivity of 66%.


- ClusterCentroids model


![image](https://user-images.githubusercontent.com/100812079/176060029-4e197264-64f2-457a-a8c3-d2924064f36b.png)

Here the balanced accuracy score is  about 51%.
The high_risk precision is still 1% only with 60% sensitivity which makes a F1 of 1%.
Due to the high number of false positives, the low_risk sensitivity is only 43%.


- SMOTEENN model

![image](https://user-images.githubusercontent.com/100812079/176060454-836b5bce-0358-4524-ac8f-045038d71545.png)

The balanced accuracy score is about 62%.
The high_risk precision is still 1% only with 71% sensitivity which makes a F1 of only 2%.
Due to the high number of false positives, the low_risk sensitivity is 53%.

- BalancedRandomForestClassifier model

![image](https://user-images.githubusercontent.com/100812079/176060585-a92f41ec-0d7e-4ea5-b343-8c9412a17308.png)

The balanced accuracy score improved to about 79%.
The high_risk precision is still low at 4% only with 67% sensitivity which makes a F1 of only 7%.
Due to a lower number of false positives, the low_risk sensitivity is now 91% with 100% presicion.

- EasyEnsembleClassifier model

![image](https://user-images.githubusercontent.com/100812079/176060617-4ca995df-69d3-48ae-85bb-6c14de1c3056.png)


The balanced accuracy score is high to about 93%.
The high_risk precision is still low at 7% only with 91% sensitivity which makes a F1 of only 14%.
Due to a lower number of false positives, the low_risk sensitivity is now 94% with 100% presicion.

## Summary: 

Credit-risk is a difficult thing to predict, even for advanced machine learning algorithms with 93 columns of data to process. All the models used to perform the credit risk analysis show weak precision in determining if a credit risk is high. The Ensemble models brought a lot more improvment specially on the sensitivity of the high risk credits. The EasyEnsembleClassifier model shows a recall of 92% so it detects almost all high risk credit.
EasyEnsembleClassifier will perform a High-Risk loan precision as a great value for the overall analysis.


I appreciate the opportunity to present this project, I am available for any clarification.



**Luiz Fernando Hoepers**  
###### UofT SCS Data Analytics Boot Camp
