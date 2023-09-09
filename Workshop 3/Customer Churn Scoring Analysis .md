# Churn Scoring

**Notebooks :** [Churn_Scoring](https://github.com/ZeroGravigra/MADT8101-Customer-Analytics/blob/c5b8ec09920fe8200742c9bba15cb068392cdf48/Homework%203%20Customer%20Churn%20Scoring/Raw%20Data/Churn_Scoring.ipynb)  
**Google Colab:** [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)]() [![](https://img.shields.io/badge/-Python-green)](#) 

## _Case Analysis_
* Dataset : Non Contractial Customers : E-Commerce Industry
* Objevtive : Identify New Customers > Active Customer > Inactive ( Window Period ) > Churn
* 


## _Methodology_
Split dataset to test set and train set, Labeling Churn in `E_COM DATASET` for ML to learn and identified the Behavior pattern of Churned Customer, finally to provide the propability score to forcast the leaving customers which can be converted beforehand.
### _ML Learning_
> ## **Logistic regression**
> 
>_OVER_SAMPLING (SMOTES TECH.)_ : For each minority class instance, SMOTE selects its k-nearest neighbors and generates synthetic examples by blending the feature vectors of the instance and its neighbors.
>>_OVER_SAMPLING_ : Randomly generates examples of instances from the majority class until the desired class balance is achieved.
>>>_UNDER_SAMPLING_ : Randomly select a subset of instances from the majority class until the desired class balance is achieved.
>
> ## **Random forest**
> 
>_OVER_SAMPLING (SMOTES TECH.)_ : For each minority class instance, SMOTE selects its k-nearest neighbors and generates synthetic examples by blending the feature vectors of the instance and its neighbors.
>>_OVER_SAMPLING_ : Randomly generates examples of instances from the majority class until the desired class balance is achieved.
>>>_UNDER_SAMPLING_ : Randomly select a subset of instances from the majority class until the desired class balance is achieved.
>
> ## **K-Nearest Neighbors**
> 
>_OVER_SAMPLING (SMOTES TECH.)_ : For each minority class instance, SMOTE selects its k-nearest neighbors and generates synthetic examples by blending the feature vectors of the instance and its neighbors.
>>_OVER_SAMPLING_ : Randomly generates examples of instances from the majority class until the desired class balance is achieved.
>>>_UNDER_SAMPLING_ : Randomly select a subset of instances from the majority class until the desired class balance is achieved.
>
> ## **XG Boost**
> 
>_OVER_SAMPLING (SMOTES TECH.)_ : For each minority class instance, SMOTE selects its k-nearest neighbors and generates synthetic examples by blending the feature vectors of the instance and its neighbors.
>>_OVER_SAMPLING_ : Randomly generates examples of instances from the majority class until the desired class balance is achieved.
>>>_UNDER_SAMPLING_ : Randomly select a subset of instances from the majority class until the desired class balance is achieved.
>
_Case Analysis_

