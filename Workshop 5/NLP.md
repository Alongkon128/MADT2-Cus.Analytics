# Voice of Customer
#### ........กระบวนการรวบรวมและทำความเข้าใจความคิดเห็น ความคิดเห็น ความชอบ และความคาดหวังของลูกค้าเกี่ยวกับผลิตภัณฑ์ บริการ หรือแบรนด์ เป็นองค์ประกอบสำคัญของการจัดการประสบการณ์ลูกค้าและการพัฒนาผลิตภัณฑ์ ช่วยให้องค์กรต่างๆ จัดข้อเสนอให้สอดคล้องกับความต้องการและความปรารถนาของลูกค้า เช่น การวิเคราะห์ 'Sentiment' ของลูกค้าที่ฝังอยู่ในข้อความและรีวิวเป็นพันๆหมื่นๆข้อความ หรือแม้กระทั้งตอบโจทย์การเพิ่ม 'Satisfaction' ของลูกค้าในการบริการที่ Realtime & Accurated มาขึ้นจาก Chatbot Intellitegent

### Benefit of LISTENING
1. **Filling in the Gaps:**
- การวิเคราะห์ VoC ช่วยระบุช่องว่างในการสื่อสาร การตลาด หรือผลิตภัณฑ์และบริการ โดยเผยให้เห็นส่วนที่ประสบการณ์ของลูกค้าไม่เป็นไปตามความคาดหวัง ทำให้เกิดการปรับเปลี่ยนและปรับปรุงได้
2. **Increasing Customer Loyalty:**
- ประสบการณ์เชิงบวกของลูกค้า ซึ่งขับเคลื่อนโดยข้อมูลเชิงลึกของ VoC ช่วยเพิ่มความภักดีของลูกค้า ผลการศึกษาพบว่าประสบการณ์ของลูกค้ามีส่วนสำคัญในการรักษาลูกค้าไว้
3. **Product Research and Development:**
- ความคิดเห็นของ VoC ให้ข้อมูลเชิงลึกที่มีคุณค่าเกี่ยวกับมุมมองของลูกค้า ช่วยให้เข้าใจประเด็นที่เป็นปัญหาและความต้องการ ข้อมูลเชิงลึกเหล่านี้เป็นแรงบันดาลใจในการปรับปรุงผลิตภัณฑ์และฟีเจอร์ ส่งเสริมการมีส่วนร่วมและความไว้วางใจของลูกค้า
4. **Crisis Management:**
- การตรวจสอบ VoC แบบเรียลไทม์ช่วยให้สามารถคาดการณ์ปัญหาเชิงรุกได้ ช่วยในการแก้ไขปัญหาต่างๆ เช่น ความผิดปกติของผลิตภัณฑ์หรือฟีเจอร์ ก่อนที่จะบานปลาย ช่วยเพิ่มชื่อเสียงของแบรนด์และความพึงพอใจของลูกค้า
### VoC Tools
* `Sentiment analysis`,`Fake review identification`,`Topic identification`,`Net promoter score` ,`Named entity recognition`
  #### Natural language processing (NLP) 
  - การประมวลผลภาษาธรรมชาติ (NLP) เป็นเทคโนโลยีแมชชีนเลิร์นนิ่งที่ช่วยให้คอมพิวเตอร์สามารถตีความ จัดการ และทำความเข้าใจภาษามนุษย์ได้ องค์กรในปัจจุบันมีข้อมูลเสียงและข้อความจำนวนมากจากช่องทางการสื่อสารต่างๆ เช่น อีเมล ข้อความ ฟีดข่าวโซเชียลมีเดีย วิดีโอ เสียง และอื่นๆ พวกเขาใช้ซอฟต์แวร์ NLP เพื่อประมวลผลข้อมูลนี้โดยอัตโนมัติ 

# Case Analysis
[![](https://img.shields.io/badge/-Python-green)](#) [![](https://img.shields.io/badge/Noises-blue)](#) [![](https://img.shields.io/badge/NLP-red)](#) 

## _'TrueMoney' Application (by 'True Money Company Limtied')_
#### ทรูมันนี่ คือแอปพลิเคชันทางการเงินที่ให้บริการครบวงจรทั้งการใช้จ่าย ออมเงินพร้อมรับดอกเบี้ย หรือแม้กระทั้งการลงทุน อีกทั้งยังสามารถใช้ 'Wallet' จ่ายแทนเงินสดได้ทั้งใช้ซื้อสินค้าที่เซเว่น-อีเลฟเว่น จ่ายบิล เติมเงินมือถือและอื่นๆ 

 <img src="https://github.com/Alongkon128/MADT2-Cus.Analytics/blob/main/Workshop%205/truefont.PNG" width="200" height="400">  <img src="https://github.com/Alongkon128/MADT2-Cus.Analytics/blob/main/Workshop%205/trueback.PNG" width="200" height="400">
### Business Objective
   - `Active Users` ลดลงจากเดิมไปเรื่อยๆจึงอยากนำข้อมูลของลูกค้าที่มีนำวิเคราะห์และประยุกต์ให้เกิดประโยชน์สูงสุด
![ProjectOverview](./Overview.png)  
### Action Plan
   - นำข้อมูล Voice of Customers หรือคอมเม้นและรีวิวของ `Active Users` และ `Non-Active Users` ล่าสุดมาวิเคราะห์เพื่อหา Sentiment และข้อที่ต้องปรับปรุงเพื่อสร้าง UX ที่ดีให้กับลูกค้าที่ใช้งาน 'TrueMoney' Application ผ่านการทำ topic modelling ML โดย  **Google Colab :** [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1X2o4aIkuh1thp0yEJWS_EmCW0VNpIsQT#scrollTo=kcPwk-oxSEUO)
### Data Strategy

28 Comments in Total reviewed on`Appstore` ขนาดไฟล์ `CSV Document - 10 KB`
* Methodology to perform topic modelling by using LDA result, VOC was divided into 4 topics
  1. Removing TH stopwords + TH Selected_words
  2. Tokenize Words
  3.  after tokenization
  4. e-wallet connection
  **Google Colab :** [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1X2o4aIkuh1thp0yEJWS_EmCW0VNpIsQT#scrollTo=kcPwk-oxSEUO)
