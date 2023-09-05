# Voice of Customer
[![](https://img.shields.io/badge/-Python-green)](#) [![](https://img.shields.io/badge/Noises-blue)](#) [![](https://img.shields.io/badge/NLP-red)](#) 

### Overview
#### ........การประมวลผลภาษาธรรมชาติ (NLP) เป็นเทคโนโลยีแมชชีนเลิร์นนิ่งที่ช่วยให้คอมพิวเตอร์สามารถตีความ จัดการ และทำความเข้าใจภาษามนุษย์ได้ องค์กรในปัจจุบันมีข้อมูลเสียงและข้อความจำนวนมากจากช่องทางการสื่อสารต่างๆ เช่น อีเมล ข้อความ ฟีดข่าวโซเชียลมีเดีย วิดีโอ เสียง และอื่นๆ พวกเขาใช้ซอฟต์แวร์ NLP เพื่อประมวลผลข้อมูลนี้โดยอัตโนมัติ วิเคราะห์ 'Sentiment' ของลูกค้าที่ฝังอยู่ในข้อความและรีวิวเป็นพันๆหมื่นๆข้อความ หรือแม้กระทั้งตอบโจทย์การเพิ่ม 'Satisfaction' ของลูกค้าในการบริการที่ Realtime & Accurated มาขึ้นจาก Chatbot Intellitegent

## Benefit LISTENING
1. Customer Profile : พร้อมข้อมูล hierarchy ของ `Downline` และ `Sponsors`
2. Transaction Logs : Sales records from year 2021 to 2022

# Natural language processing (NLP) 
การประมวลผลภาษาธรรมชาติ (NLP) เป็นเทคโนโลยีแมชชีนเลิร์นนิ่งที่ช่วยให้คอมพิวเตอร์สามารถตีความ จัดการ และทำความเข้าใจภาษามนุษย์ได้ องค์กรในปัจจุบันมีข้อมูลเสียงและข้อความจำนวนมากจากช่องทางการสื่อสารต่างๆ เช่น อีเมล ข้อความ ฟีดข่าวโซเชียลมีเดีย วิดีโอ เสียง และอื่นๆ พวกเขาใช้ซอฟต์แวร์ NLP เพื่อประมวลผลข้อมูลนี้โดยอัตโนมัติ วิเคราะห์ 'Sentiment' ของลูกค้าที่ฝังอยู่ในข้อความและรีวิวเป็นพันๆหมื่นๆข้อความ หรือแม้กระทั้งตอบโจทย์การเพิ่ม 'Satisfaction' ของลูกค้าในการบริการที่ Realtime & Accurated มาขึ้นจาก Chatbot Intellitegent 
- `Payment_date` ที่นำมาวิเคราะห์ระหว่าง "01 July 22" - "01 June 23"

![ProjectOverview](./Overview.png)   

# 1) Create single customer view
#### Features 36 Viables : No., Field name, Meaning
* `member_id` : Define “ent” from member data as primary key
* `original_status` : -
* `sponsorship` : Influential power
* `registered_year` : Starting year of being  member 
* `registered_month` : Starting month of being  member 
* `member_duration` : Membership age since starting until current
* `no_of_purchasing` : Number of purchasing (Ticket counted)
* `total_spending` : Sum of sales amount
* `avg_spending` : Average total_spending per Ticket
* `total_product_qty` : Sum product quantity
* `total_product_qty_bycategory` : Sum product quantity by category (26 category)
* `category_count` : Count purchased category
* `sku_count` : Count purchased sku
* `Percent_paid` : Paid/Total_spending
* `avg_paid` : Percent_paid/no_of_purchasing
* `MTBP_Days` : (Last purchased-First purchased)/no. of purchasing
* `NO_CAT_rank` : Percentile of number of purchasing by category (26 category)
* `Percent_no_online` : total online transactions/total transactions

# 2) Customer Segmentation
### K-Mean Clustering
การแบ่งกลุ่มโดยใช้การ algorithm K-Mean เป็นเทคนิคการวิเคราะห์ข้อมูลที่จัดกลุ่มจุดข้อมูลที่คล้ายคลึงกันเข้าไว้ด้วยกันเป็นกลุ่ม การจัดกลุ่มเคมีนสามารถนำไปใช้เพื่อระบุกลุ่มลูกค้าที่แตกต่างกันตามพฤติกรรมการซื้อหรือความชอบของพวกเขา ช่วยให้ธุรกิจสามารถสร้างคำแนะนำผลิตภัณฑ์เป้าหมายสำหรับแต่ละ Cluster ได้ 

### K-Mean Methodology
การจัดกลุ่มแบบ K-Mean ทำงานโดยการกำหนดจุดข้อมูลซ้ำๆ ให้กับเซนทรอยด์ของคลัสเตอร์ที่ใกล้ที่สุด จากนั้นคำนวณเซนทรอยด์ใหม่ตามจุดที่ได้รับมอบหมาย กระบวนการนี้จะดำเนินต่อไปจนกว่าเซนทรอยด์จะเสถียรและเกิดกระจุกขึ้น _aims to minimize the sum of squared distances between data points and their respective cluster centroids_

## Workflow Overview
![Kmean-Clustering](./Kmean.png)  
* หลังจากการทำ K-Mean รอบแรกด้วย K=3 ทำให้ได้ออกมาเป็น 3 Cluster ใหญ่ๆ
  
1. Shopper Elite
   - `AGV Spending` 1.2 M ,`AGV SKU` 3.66 K,`AGV MTBT/Days` 126.36 K
2. Product Lover
   - `AGV Spending` 195.4 K ,`AGV SKU` 28.15 K,`AGV MTBT/Days` 14.61 K
3. General Shopper
   - _Begin to Clustering 2st round the propotion stand more than 65.74%_

![FirstGroup](./first.png) 

* "General Shopper" นำมาทำ K-Mean รอบที่สองโดย K=3 ทำให้ได้ 3 Cluster ออกมาอีกในการวิเคราะห์
  
1. Shopper Loyalist
   - `AGV Spending` 514.1 K ,`AGV SKU` 7.04 K,`AGV MTBT/Days` 26.31 K
2. Need Attention
   - `AGV Spending` 231.5 K ,`AGV SKU` 4.51 K,`AGV MTBT/Days` 64.09 K
3. Product Leader
   - `AGV Spending` 153 K ,`AGV SKU` 10.51 K,`AGV MTBT/Days` 21.11 K
   
![SecondGroup](./second.png) 


* จากกลุ่มทั้งหมด 5 กลุ่มที่ผ่านการ Clustering 2 รอบเราได้เลือก 2 กลุ่มขึ้นมายกตัวอย่างในการทำ Analyses ต่อโดยใช้ Collaborative Filtering เพื่อค้นหาและแนะนำสินค้าที่มีความเป็นไปได้สูงว่าลูกค้าในกลุ่มเดียวกันจะสนใจโดยจุดประสงค์เพื่อ เพิ่มยอดขายจากการทำ Campaign ที่ผ่านการตัดสินจากข้อมูลที่มี
  
1. Shopper Loyalist
   - `AGV Spending` 514.1 K ,`AGV SKU` 7.04 K,`AGV MTBT/Days` 26.31 K
2. Shopper Elite
   - `AGV Spending` 1.2 M ,`AGV SKU` 3.66 K,`AGV MTBT/Days` 126.36 K
     
![PotentialGroup](./Potential.png) 

### Collaborative Filtering
Item-Based Collaborative Filtering: In this approach, items are compared based on their interactions with users. Items that are frequently interacted with by the same group of users are considered similar.

![Collabolative](./Collabo.png)   
![Recommended Products](./Productrec.png) 
