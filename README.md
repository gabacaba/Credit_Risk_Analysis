# Credit_Risk_Analysis

## Overview
The following assignment uses machine learning models to determine the credit card risk of loan applicants. The assignment uses the imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. It also uses six algorithms: RandomOverSampler, SMOTE, ClusterCentroids, SMOTENN, BalancedRandomForestClassifier and EasyEnsembleClassifier. This with the purpose to predict credit risk. 
Below you can find the results of using the above mentioned models as well as an evaluation of the performance of these models.

## Results

- **RandomOverSampler** 
The Balanced accuracy score is 0.6441747142552103 - 65%
The Precision score for the high risk is 0.01 - 1% with 0.62 - 62% recall score. The f1 is 0.02 - 2%.
The precision score for the low risk is 1.00 - 100% with a recall score of 0.68 - 68%. 
![RANDOMOVERSAMPLER MODEL](https://user-images.githubusercontent.com/88411140/144346719-cbd91ef9-b905-40ac-a562-35e53f0a0423.png)

- **SMOTE**
The Balanced accuracy score is 0.6482720346801714 - 65%
The Precision score for the high risk is 0.01 - 1% with 0.66 - 66% recall score. The f1 is 0.02 - 2%.
The precision score for the low risk is 1.00 - 100% with a recall score of 0.64 - 64%. 
![SMOTE MODEL](https://user-images.githubusercontent.com/88411140/144346781-1397d904-46da-4c5d-9aae-db681fdffa0a.png)

- **ClusterCentroids** 
The Balanced accuracy score is 0.5298576614251584 - 53%
The Precision score for the high risk is 0.01 - 1% with 0.61 - 61% recall score. The f1 is 0.01 - 1%.
The precision score for the low risk is 0.99 - 99% with a recall score of 0.45 - 45%. 
![ClusterCentroids](https://user-images.githubusercontent.com/88411140/144346802-aff9e973-e174-4c10-82fa-153c4c388346.png)

- **SMOTENN**
The Balanced accuracy score is 0.6235037931437366 - 62%
The Precision score for the high risk is 0.01 - 1% with 0.70 - 70% recall score. The f1 is 0.02 - 2%.
The precision score for the low risk is 1.00 - 100% with a recall score of 0.55 - 55%. 
![SMOTENN MODEL](https://user-images.githubusercontent.com/88411140/144346849-3dc5bbc2-ea3b-410a-8613-ae81aaca836d.png)

- **BalancedRandomForestClassifier**
The Balanced accuracy score is 0.7877672625306695- 78%
The Precision score for the high risk is 0.04 - 4% with 0.67 - 67% recall score. The f1 is 0.07 - 7%.
The precision score for the low risk is 1.00 - 100% with a recall score of 0.91 - 91%. 
![BALANCEDRANDOMFOREST MODEL](https://user-images.githubusercontent.com/88411140/144346892-54def3a7-353c-48d4-8618-411ecbfa4cb4.png)

- **EasyEnsembleClassifier**
The Balanced accuracy score is 0.925427358175101- 92%
The Precision score for the high risk is 0.07 - 7% with 0.91 - 91% recall score. The f1 is 0.14 - 14%.
The precision score for the low risk is 1.00 - 100% with a recall score of 0.94 - 94%. 
![EASYENSEMBLE MODEL](https://user-images.githubusercontent.com/88411140/144346907-56463f2d-ecfa-4983-9495-2fe3eaa50fe6.png)

## Summary: 

### Results Summary 
The results show the precision, recall and F1 score of each model's performance. This helps to determine how well the model works to predict credit risk. 

The accuracy of the models lays between 53% to 92%. The best accuracy score is the EasyEnsembleClassifier model with 92%.  

The precision tells how likely is the credit risk to be true or how reliable is a positive classification. The precision score of the first four high risk models is 0.01 or 1%, and the precision score of low risk is 100%. The precision score of the last two models is BalancedRandomForestClassifier high risk 4% and EasyEnsembleClassifier high risk 7%. 

The sensitivity of the model, also known as recall, is a measurement that says of the people who have credit risk, how many were detected. The recall score for high risk lays between 61% and 91%, and for low risk 45% to 94%. The EasyEnsembleClassifier obtained the best recall scores.  

### Recomendations

The accuracy score of the first 4 models is quite low (below 70%). This could be because of the imbalance nature of the sample. Meaning that the first four models are good at determine low risk and bad at determine high risk. However, the accuracy score of the last two models where we resampled the data using ensemble classifier was better (above 78%). 

In terms of the precision score, the first four models show a weak precision regarding high credit risk. The last two models show an improved precision score, 4% and 7% versus 1%.

In terms of the sensitivity or recall score, the last two models also show the best scores. 

The EasyEnsembleClassifier therefore shows a high accuracy, low precision and high recall scores. Which means that it has a good detection capability but there's also the risk of false positives. 

Even though none of the models is perfect, the bank could use either the EasyEnsembleClassifier model or BalanceRandomForest classifier because are better balanced than the other models. 
