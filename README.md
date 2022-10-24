# Credit_Risk_Analysis

## Overview of the analysis
 
For this project, I was tasked with employing different techniques to train and evaluate models with unbalanced classes. I utilized the imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. I oversampled data using the RandomOverSampler and SMOTE algorithms and also undersampled data using the ClusterCentroids algorithm. I used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm and compared two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

## Results
 
For this project, I employed 6 machine learning models. To determine performance, we will look at 3 things: balanced accuracy score, precision, and recall score. 

Accuracy is one way to assess a model's performance. It shows you what percentage of predictions the model got right. Achieving an accuracy score of 1.0 indicates that the model correctly predicted every observation in the testing set. Precision, also known as positive predictive value (PPV), is a measure of how likely something is. Lastly, a test with high Recall or Sensitivity indicates few false negatives, however there could be a high number of false positives within the testing set.

Below is the Random Oversampler method. Looking at the balanced accuracy score, the precision, and recall score, we see the following:
* Balanced accuracy score
	* .6366
* Precision 
	* .99
* Recall score
	* .65

![RandomOverSamplerMLM](https://github.com/billy-bartlett/Credit_Risk_Analysis/blob/main/Resources/RandomOverSamplerMLM.png?raw=true)

Below is the SMOTE method.
* Balanced accuracy score
	* .6375
* Precision 
	* .99
* Recall score
	* .57

![SmoteMLM](https://github.com/billy-bartlett/Credit_Risk_Analysis/blob/main/Resources/SmoteMLM.png?raw=true)

Below is the ClusterCentroids method.
* Balanced accuracy score
	* .6302
* Precision 
	* .99
* Recall score
	* .44

![ClusterCentroidsMLM](https://github.com/billy-bartlett/Credit_Risk_Analysis/blob/main/Resources/ClusterCentroidsMLM.png?raw=true)

Below is the SMOTEENN method.
* Balanced accuracy score
	* .5160
* Precision 
	* .99
* Recall score
	* .57

![SMOTEENNMLM](https://github.com/billy-bartlett/Credit_Risk_Analysis/blob/main/Resources/SMOTEENNMLM.png?raw=true)

Below is the Balanced Random Forest Classifier method. 
* Balanced accuracy score
	* .7877
* Precision 
	* .99
* Recall score
	* .91

![BalancedRandomForestClassifierMLM](https://github.com/billy-bartlett/Credit_Risk_Analysis/blob/main/Resources/BalancedRandomForestClassifierMLM.png?raw=true)

Below is the Easy Ensemble Classifier method. 
* Balanced accuracy score
	* .9254
* Precision 
	* .99
* Recall score
	* .94

![EasyEnsembleClassifierMLM](https://github.com/billy-bartlett/Credit_Risk_Analysis/blob/main/Resources/EasyEnsembleClassifierMLM.png?raw=true)

## Summary: 
The models with the highest accuracy were the Easy Ensemble Classifier (.9254) and the Balanced Random Forest Classifier (.7877). All models had a high precision coming in at .99 for all models. The models with the highest recall scores were the Easy Ensemble Classifier (.94) and the Balanced Random Forest Classifier (.91). 

The best overall model to use is the Easy Ensemble Classifier Model. This model correctly predicted predictions 92.54% of the time and had a precision of .99. It also has a recall score of .94 indicating there are few false negatives. 



