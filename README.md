# Credit_Risk_Analysis

## Overview of the analysis: Explain the purpose of this analysis.
- The purpose of this is to use various different models to predict the outcome of credit risks using data gathered from 2019Q1 from Lending Club. First the data was oversampled using RandomOverSampler and SMOTE. Next, ClusterCentroids algothrithm was used to undersample the data set. Then, SMOTEENN alogrithm was used as a combinatorial approach to both over- and undersample the dataset. BalancedRandomForestClassifier and EasyEnsembleClassifier are the two machine learning models that are used to apply to dataset to reduce bias and predict the overall credit risk. The performances of each model was then evaluated in terms of accuracy scores and precisions. 

## Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

 ### 1. Oversample with RandomOverSampler

![RandomOverSampler](https://github.com/jhuang2801/Credit_Risk_Analysis/blob/main/Resources/RandomOverSampler.png)

RamdomOverSample result shows accuracy score of 65%.
For "high risk" prediction, this model shows precision is 1%, recall rate of 71%, and F1 score of 2%.

### 2. Oversample with SMOTE

![SMOTE Oversample](https://github.com/jhuang2801/Credit_Risk_Analysis/blob/main/Resources/SMOTEOversampling.png)

SMOTE result shows accuracy score of 66%.
For "high risk" prediction, this model shows precision of 1%, recall rate of 63%, and F1 score of 2%.

### 3. Undersample with ClusterCentroid

![ClusterCentroid](https://github.com/jhuang2801/Credit_Risk_Analysis/blob/main/Resources/ClusterCentroid.png)

ClusterCentroid result shows accuracy score of 54%.
For "high risk" prediction, this model shows precision of 1%, recall rate of 69%, and F1 score of 1%.

### 4. Resample with SMOTEENN 

![SMOTEENN](https://github.com/jhuang2801/Credit_Risk_Analysis/blob/main/Resources/SMOTEENN.png)

SMOTEENN result shows accuracy score of 64%.
For "high risk" prediction, this model shows precision of 1%, recall rate of 68%, and F1 score of 2%.

### 5. Resample with BalancedForestClassifier

![BalancedForestClassifier](https://github.com/jhuang2801/Credit_Risk_Analysis/blob/main/Resources/BalancedForestClassifier.png)

BalancedForestClassifer result shows accuracy score of 79%.
For "high risk" prediction, this model shows precision of 3%, recall rate of 70%, and F1 score of 6%.

### 6. Resample with EasyEnsembleClassifier

![EasyEnsembleClassifier](https://github.com/jhuang2801/Credit_Risk_Analysis/blob/main/Resources/EasyEnsembleClassifier.png)

EasyEnsembleClassifier result shows accuracy score of 93%.
For "high risk" prediction, this model shows precision of 9%, recall rate of 92%, and F1 score of 16%.

## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

EasyEnsemble would be the recommended model to use. It has the highest accuracy % at 93 %, and the most balanced precision, recall, and F1 scores. SMOTEENN model would not be recommended similarly for its low accuracy scores, and low precision/recall/F1 values. 

