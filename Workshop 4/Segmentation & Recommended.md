# Customer Segmentation to Product Recommended
[![](https://img.shields.io/badge/-Python-green)](#) [![](https://img.shields.io/badge/-K--Means-orange)](#) [![](https://img.shields.io/badge/-Collaborative--Filtering-orange)](#) 

# Overview
![ProjectOverview](./img/ProjectOverview.PNG)
# Data Set
![ProjectOverview](./img/ProjectOverview.PNG)

1. data member : master data of downline and his/her sponsor
2. transaction 2021 - 2022 : contains sales by bill from year 2021 to 2022
#### Created Dataset
1. sponsor master : master data of sponsor and no. of downline per sponsor
2. salesbyitem 2021 - 2022 : extract json product file to sales quantiy by item

# 2) Create single customer view
base on datasets above, we create the following data single customer view table:      

![SCV](./img/SCV.png)     

- List of SCV Features
  
![feature](./img/feature.PNG)

# 3) Clustering
**Notebooks:** [Clustering Model](./V2_1_HDI_Segmentation.ipynb)  
**Google Colab:** [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jane-russ/MADT8101/blob/main/5.Segmentation/V2_1_HDI_Segmentation.ipynb)
#### Features
All the features are taken from single customer view table
#### Choosing K number of clusters
Choose `K = 4` with the lowest silhoette score of 0.26
![choosingK](./img/choosingK.PNG)

#### Clustering Result
![clustering_result](./img/clusterplot.png)
