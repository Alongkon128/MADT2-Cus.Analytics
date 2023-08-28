# Customer Segmentation to Product Recommended
[![](https://img.shields.io/badge/-Python-green)](#) [![](https://img.shields.io/badge/-K--Means-orange)](#) [![](https://img.shields.io/badge/-Collaborative--Filtering-orange)](#) 

# Overview
#### ........การทำ Segmentation คือ การแบ่งฐานผู้บริโภคในวงกว้างออกเป็นกลุ่มต่างๆ ตามคุณลักษณะหรืแที่มีร่วมกันตามตัวแปรที่เชื่อว่าเป็น Key Measure  เมื่อระบุกลุ่มเหล่านี้แล้ว จะสามารถสร้างคำแนะนำผลิตภัณฑ์ที่เหมาะกับแต่ละกลุ่มได้ User-Based (Collaborative-Filtering) ด้วยการทำความเข้าใจความต้องการและความชอบเฉพาะตัวของกลุ่มธุรกิจเหล่านี้ จึงสามารถเสนอ Recommend System ที่ตรงใจลูกค้าได้ดียิ่งขึ้นและการันตีการเพิ่มยอดขายให้แก่องค์กร

![ProjectOverview](./Overview.png)
# Data Set
![ProjectOverview](./img/ProjectOverview.PNG)

1. data member : Customer Profile พร้อมข้อมูล hierarchy ของ 'downline' และ 'sponsor'
2. transaction 2021 - 2022 : contains sales by bill from year 2021 to 2022
#### Created Dataset
1. sponsor master : master data of sponsor and no. of downline per sponsor
2. salesbyitem 2021 - 2022 : extract json product file to sales quantiy by item

# 2) Create single customer view
base on datasets above, we create the following data single customer view table:      

![SCV](./img/SCV.png)     


# 1) ระบุเกณฑ์การแบ่งส่วน

เริ่มต้นด้วยการระบุเกณฑ์ที่คุณจะใช้เพื่อแบ่งกลุ่มตลาดของคุณ สิ่งเหล่านี้อาจรวมถึงปัจจัยทางประชากร (อายุ เพศ รายได้) ปัจจัยทางจิต (ไลฟ์สไตล์ ค่านิยม ความสนใจ) ปัจจัยด้านพฤติกรรม (ประวัติการซื้อ พฤติกรรมออนไลน์) หรือปัจจัยทางภูมิศาสตร์ (สถานที่ สภาพภูมิอากาศ) เกณฑ์ที่คุณเลือกควรเกี่ยวข้องกับผลิตภัณฑ์ของคุณและเป้าหมายของกลยุทธ์การแนะนำของคุณ


**Notebooks:** [Clustering Model](./V2_1_HDI_Segmentation.ipynb)  
**Google Colab:** [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jane-russ/MADT8101/blob/main/5.Segmentation/V2_1_HDI_Segmentation.ipynb)
#### Features
All the features are taken from single customer view table
#### Choosing K number of clusters
Choose `K = 4` with the lowest silhoette score of 0.26
![choosingK](./img/choosingK.PNG)

#### Clustering Result
![clustering_result](./img/clusterplot.png)
