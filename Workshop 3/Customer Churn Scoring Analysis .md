#Churn Scoring
[![](https://img.shields.io/badge/-Classification-orange)](#) [![](https://img.shields.io/badge/-Python-green)](#) 
**Google Colab:** [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)]()

## Data Processing
**Notebooks :** [Churn_Scoring](https://github.com/ZeroGravigra/MADT8101-Customer-Analytics/blob/c5b8ec09920fe8200742c9bba15cb068392cdf48/Homework%203%20Customer%20Churn%20Scoring/Raw%20Data/Churn_Scoring.ipynb)  
**Google Colab :** [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ZeroGravigra/MADT8101-Customer-Analytics/blob/main/Homework%203%20Customer%20Churn%20Scoring/Raw%20Data/Churn_Scoring.ipynb)

# _Methodology_
* Split dataset to test set and train set, Labeling Churn in `E_COM DATASET` for ML to learn and identified the Behavior pattern of Churned Customer, finally to provide the propability score to forcast the leaving customers which can be converted beforehand.
>_OVER_SAMPLING (SMOTES TECH.)_ : For each minority class instance, SMOTE selects its k-nearest neighbors and generates synthetic examples by blending the feature vectors of the instance and its neighbors.
>>_OVER_SAMPLING_ : Randomly generates examples of instances from the majority class until the desired class balance is achieved.
>>>_UNDER_SAMPLING_ : Randomly select a subset of instances from the majority class until the desired class balance is achieved.


_Case Analysis_

