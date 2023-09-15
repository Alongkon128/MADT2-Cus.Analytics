# Churn Scoring
"Churn" typically refers to the rate at which customers or subscribers **stop** using a product or service, often in the context of businesses or subscription-based services. Churn is usually expressed as a percentage called "Churn Rate". By analyzing the rate of churn, we can figure out how to retain more customers byimproving UX, optimizing features, adjusting prices, give away promotions at specific of time. Analyzing method which use in ganeral called "Cohort Analysis" oftenly used by analysis team.


![Churn Rate](./Churnrate.webp)
Reference : _https://www.adjust.com/glossary/churn-definition/_

## _Cohort Analysis_
Wording "cohort" means a group of individuals who share a common characteristic or experience within a defined time frame. The most popular used in Marketing area would be : 

* "Customers Acquisition", a customer to be a grouped as New customers who made their first purchase in a specific month or quarter, then analyzing the spending behavioro over time in order to gain the insight such `Retention Rate` `Customer lifetime value` `Customer lifespan`.  


![Cohort](./cohortanalysis.webp)
Reference : _https://mode.com/blog/cohort-analysis-helps-look-ahead/_

## _Case Analysis_
[![](https://img.shields.io/badge/-Python-green)](#)   **Notebooks :** [Churn_Scoring](https://github.com/Alongkon128/MADT2-Cus.Analytics/blob/main/Workshop%203/Churn_scoring.ipynb)  
* Dataset : Non Contractial Customers : E-Commerce Industry
* Objevtive : Perform Feature Engineering to identify the importance viaribles, before go to machine learning
_New Customers > Active Customer > Inactive ( Window Period ) > Churn_


## _Methodology_
Split dataset to test set and train set, Labeling Churn in `E_COM DATASET` for ML to learn and identified the Behavior pattern of Churned Customer, finally to provide the propability score to forcast the leaving customers which can be converted beforehand.


### _ML Learning_

![Models](./Models.png)

![Sampling Methods](./Sampling.png)

> ## **Logistic regression**
> 
>_OVER_SAMPLING (SMOTES TECH.)_ : For each minority class instance, SMOTE selects its k-nearest neighbors and generates synthetic examples by blending the feature vectors of the instance and its neighbors.
>>_OVER_SAMPLING_ : Randomly generates examples of instances from the majority class until the desired class balance is achieved.
>>>_UNDER_SAMPLING_ : Randomly select a subset of instances from the majority class until the desired class balance is achieved.
>
> ## **Random forest**
> 
>_OVER_SAMPLING (SMOTES TECH.)_
>>_OVER_SAMPLING_ 
>>>_UNDER_SAMPLING_ 
>
> ## **K-Nearest Neighbors**
> 
>_OVER_SAMPLING (SMOTES TECH.)_
>>_OVER_SAMPLING_ 
>>>_UNDER_SAMPLING_ 
>
> ## **XG Boost**
> 
>_OVER_SAMPLING (SMOTES TECH.)_
>>_OVER_SAMPLING_ 
>>>_UNDER_SAMPLING_ 
>

### _Result Model Scoring_
![Ranking Score](./Score.png)

