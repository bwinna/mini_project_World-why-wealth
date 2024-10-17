
## Project : Life Expectancy Analysis

Mini-Project นี้เป็นส่วนหนึ่งของวิชา DADS5001: Data Analytics and Data Science Tools and Programming

## จัดทำโดย

- 6610422015 นายชานุกฤต วรรณวัฒน์
- 6620422026 นางสาววิญณา บางสร้อย

คําอวยพรที่ว่า “ขอให้สุขภาพแข็งแรง อายุยืนยาว” สะท้อนให้เห็นว่ามนุษย์เรานั้นให้ความสําคัญกับการที่จะมีอายุยืนยาวมากแค่ไหน โดย Projectนี้ จะทำการศึกษาปัจจัยที่ส่งผลต่ออายุขัยเฉลี่ยของมนุษย์ ความสัมพันธ์ระหว่างอายุขัยกับความสุข ตลอดจนศึกษาโครงสร้างประชากรของประเทศไทย 

อายุขัยเฉลี่ย (Life Expectancy) คือระยะเวลาโดยเฉลี่ยมีหน่วยเป็นปี ที่ประชากรกลุ่มหนึ่งจะดํารงชีวิตอยู่ได้ นับตั้งแต่เกิดไปจนกระทั่งเสียชีวิต ซึ่งค่าเฉลี่ยของประชากรแต่ละกลุ่มก็จะแตกต่างกันออกไปโดยปัจจัยและสาเหตุที่ต่างกัน ประชากรส่วนหนึ่งเกิดมาไม่นานก็เสียชีวิต บางส่วนเสียชีวิตในวัยหนุ่มสาว และบางส่วนก็เสียชีวิตเพราะความชราหรือสูงอายุนั่นเอง


## Dataset
1. Life Expectancy (2000 - 2015)
https://www.kaggle.com/datasets/lashagoch/life-expectancy-who-updated

3. World Happiness Report (2008 - 2023)
https://worldhappiness.report/

5. จำนวนการเกิด จำนวนการตาย จำนวนประชากรของประเทศไทย (2002 - 2023)
https://stat.bora.dopa.go.th/stat/statnew/statMenu/newStat/home.php

7. งบประมาณของประเทศไทย (2016 - 2022)
https://govspending.data.go.th

9. GDP (CVM)
https://www.nesdc.go.th/main.php?filename=qgdp_page

- [Data difinition](difinition.md)
  
## Question 
1. ประมาณการอายุขัย (life expectancy) ของประชากรโลกเป็นอย่างไร

2. ปัจจัยอะไรบ้างที่ส่งผลต่อประมาณการอายุขัยเฉลี่ย และส่งผลอย่างไร

3. มีเหตุการณ์ใดบ้างที่อาจส่งผลต่อประมาณการอายุขัย

4. ปัจจัยอะไรบ้างที่ส่งผลต่อความสุข (Happiness)

5. ประมาณการอายุขัยและความสุข มีความสัมพันธ์กันหรือไม่ อย่างไร

6. นำข้อมูลมาใช้ประโยชน์กับประเทศไทยได้อย่างไรบ้าง



## Question 1: ประมาณการอายุขัยเฉลี่ย (Life Expectancy) ในปี 2000 - 2015 เป็นอย่างไร

### 1.1 ประมาณการอายุขัยเฉลี่ยทุกประเทศ

จากการ Research Data ที่ World Health Organization ได้เก็บรวบรวมประมาณการของอายุขัยเฉลี่ย (“อายุขัยฯ”) ของทุกประเทศตั้งแต่ปี 2000 ถึง 2015  พบว่ามีแนวโน้มค่อยๆ เพิ่มสูงขึ้น โดยในปี 2000 อายุขัยเฉลี่ยฯ เท่ากับ 66.4 ปี และค่อยๆ เพิ่มขึ้นเป็น 71.5 ปีในปี 2015 คิดเป็น 7.68% หรือ 0.48% ต่อปี  

สำหรับประเทศไทยพบว่ามีอายุขัยเฉลี่ยฯ สูงกว่าค่าเฉลี่ยของทั้งโลก โดยมีอายุขัยเฉลี่ยในปี 2000 เท่ากับ 70.6 ปี และเพิ่มขึ้นเป็น 76.1 ปี ในปี 2015 คิดเป็น 7.79% หรือ 0.49% ต่อปี  

**กราฟ 1:** Life Expectancy Trendline of All Countries

![image](https://github.com/user-attachments/assets/4875115b-07f4-4c20-a96c-9117ad708a3b)

### 1.2 ประมาณการอายุขัยของแต่ละทวีป

เมื่อเราแบ่งอายุขัยฯตามทวีป พบว่า ทุกทวีปมีแนวโน้มที่จะอายุขัยเพิ่มขึ้น โดย:

- **Africa** มีอัตราการเพิ่มขึ้นของอายุขัยสูงที่สุด โดยเพิ่มขึ้นจาก 54.1 ปีในปี 2000 เป็น 62.5 ปี ในปี 2015 หรือคิดเป็น 15.4%
- **Europe** และ **North America** มีอายุขัยฯเฉลี่ยสูงที่สุด แต่มีอัตราการเพิ่มขึ้นของอายุขัยต่ำกว่าเมื่อเทียบกับ **Asia** และ **Africa**

**กราฟ 2:** Life Expectancy Trendline by Region
![image](https://github.com/user-attachments/assets/062c98eb-5f6c-473b-898b-02e0a2def86c)

เมื่อพิจารณา **กราฟที่ 3** แสดงอายุขัยที่สูงที่สุด 5 อันดับในแต่ละทวีป จะเห็นได้ว่าทุกทวีปจะมีแนวโน้มที่อายุขัยเพิ่มขึ้น แต่ก็มีการกระจายที่แตกต่างกันออกไป เช่น:

- **Europe** จะมีอายุขัยเฉลี่ยสูงที่สุดและเส้นอายุขัยมีการกระจุกตัวกัน
- **North America** มีลักษณะการกระจายตัวคล้ายกับ Europe ยกเว้น **Canada** ที่มีอายุขัยสูงกว่าประเทศอื่นๆ
- **Asia** มีการกระจายตัวมากกว่า
- **Oceania** มีการแบ่งออกเป็น 2 กลุ่มชัดเจน
- **Africa** มีการเกาะกลุ่มกันแต่อายุขัยเฉลี่ยต่ำกว่าทวีปอื่นๆ

**กราฟ 3:** Top 5 Countries with the Highest Life Expectancy by Region
![image](https://github.com/user-attachments/assets/5ac4f531-59d9-48c6-87ad-c8a242024ebf)





### 1.3 ประมาณการอายุขัยของประเทศที่พัฒนาแล้วกับกำลังพัฒนา

จาก **กราฟที่ 4** และ **กราฟที่ 5** จะเห็นได้ว่า:


- กลุ่มประเทศที่พัฒนาแล้วมีอายุขัยเฉลี่ยสูงกว่ากลุ่มประเทศที่กำลังพัฒนาอย่างชัดเจน
- บางทวีปเช่น **Africa** และ **South America** มีเฉพาะประเทศที่กำลังพัฒนา ดังนั้นปัจจัยทางเศรษฐกิจก็อาจจะมีส่วนทำให้อายุขัยของประชากรเพิ่มขึ้น

**กราฟ 4:** Life Expectancy in Developed and Developing Countries by Region
![image](https://github.com/user-attachments/assets/bcbd44b5-955d-4f75-8376-11187dba86d9)

**กราฟ 5:** Life Expectancy in Developed and Developing Countries
![image](https://github.com/user-attachments/assets/521d481f-c548-4b95-84f4-6be98dacc6fa)


### 1.4 อัตราเพิ่มขึ้นของอายุขัยเปรียบเทียบกับอายุขัย
จากกราฟที่ 6 จะเห็นได้ว่า กลุ่มประเทศที่อายุขัยต่ำกว่าค่าเฉลี่ย (70.9 ปี) จะมีอัตราการเพิ่มขึ้นของอายุขัยสูงกว่ากลุ่มประเทศที่อายุขัยสูงกว่าค่าเฉลี่ย

**กราฟ 6 :**  Life Expectency Growth Rate (%) and Life Expectancy
![image](https://github.com/user-attachments/assets/49182d92-d6fc-44c7-a01a-ddc08f2547c9)



## Question 2 : ปัจจัยอะไรบ้างที่ส่งผลต่อประมาณการอายุขัยเฉลี่ย และส่งผลอย่างไร
### 2.1 อายุขัยของแต่ละประเทศเฉลี่ยใน 5 ปี (2011-2015)
ประเทศที่อายุขัยเฉลี่ยใน 5 ปี (2011-2015) สูงสุด 10 อันดับ ได้แก่ Japan, Switzerland, Spain, Iceland, Italy, France, Singapore, Australia, Sweden และ israel โดยอยู่ระหว่าง 81.96 - 83.28 ปี
ส่วนประเทศที่อายุขัยเฉลี่ย ต่ำสุด 10 อันดับ ได้แก่ Lesotho, Central African Republic, Sierra Leone, Eswatini, Nigeria, Chad, Cote d’Ivorie, Mozambique, Somalia, Guinea-Bissau โดยอยู่ระหว่าง 48.64 - 56.08 ปี
ขณะที่อายุขัยเฉลี่ยของประชากรทั้งโลกเท่ากับ 70.9 ปี และประเทศไทยออยู่อันดับที่ 58 อายุขัยเฉลี่ยประมาณ 75.36 ปี 

**กราฟที่ 7 :** Average Life Expectation by Countries (2011-2015)
![image](https://github.com/user-attachments/assets/3560b13c-d48a-49d7-b70c-4b6d069e0c19)


### 2.2 ปัจจัยที่ส่งผลต่อประมาณการอายุขัยเฉลี่ย
ปัจจัยที่สัมพันธ์กับอายุขัยมากที่สุด คือ ระยะเวลาการศึกษา (Schooling) ปัจจัยด้านสุขภาพได้แก่การครอบคลุมการได้รับวัคซีนป้องกันโรค เช่น Polio หรือ Diphtheria tetanus toxoid เป็น และปัจจัยทางเศรษฐกิจ (GDP) ในขณะที่อัตราการตายตั้งแต่ช่วงทารก การตายในเด็กไม่เกิน 5 ขวบ และการตายในวัยผู้ใหญ่มีผลทำให้อายุขัยลดลง นอกจากนี้พบว่า จำนวนประชากร ไม่ได้สัมพันธ์กันกับอายุขัย

**กราฟ 8 :** Correlation Between Factors and Life Expectancy
![image](https://github.com/user-attachments/assets/39562adf-18df-4f3e-9e7e-47c66da57361)

**กราฟ 9 :** Correlation Matrix (Life Expectancy)
![image](https://github.com/user-attachments/assets/77cf4f74-b571-4f09-8d5f-6aa72c7e1e8e)


## Question 3 : มีเหตุการณ์ใดบ้างที่อาจส่งผลต่อประมาณการอายุขัย
### 3.1 Subprime crisis
ใน USA เกิดวิกฤตเหตุการณ์ทางการเงิน Subprime crisis ปี 2008 แต่เมื่อพิจารณาจากอัตราการเพิ่มขึ้นของอายุขัยต่อปีของช่วงเวลาก่อนและหลัง พบว่าอัตราการเพิ่มขึ้นของอายุขัยต่อปีลดลงจาก 0.24% เหลือ 0.19% 

**กราฟ 10 :** USA's Life Expectancy and the Subprime Crisis
![image](https://github.com/user-attachments/assets/b5c1a0c9-cf45-43c5-ba52-0cd1acd07572)

### 3.2 SARS
การระบาดของโรคซาร์ส (Severe Acute Respiratory Syndrome) ในจีนเริ่มขึ้นในเดือนพฤศจิกายน 2002 ที่มณฑลกวางตุ้ง ก่อนที่จะแพร่ระบาดออกไปที่อื่น เมื่อพิจารณาจากอัตราการเพิ่มขึ้นของอายุขัยต่อปีของช่วงเวลาก่อนและหลัง พบว่าอัตราการเพิ่มขึ้นของอายุขัยต่อปีลดลงจาก 0.695% เหลือ 0.352% 

**กราฟ 11 :** China's Life Expectancy and SARS

![image](https://github.com/user-attachments/assets/7414c140-c2b9-4299-a3cc-a89fdab88193)

### 3.3 Afghanistan Wars (2001–2014)
หลังเหตุการณ์ 9/11 สหรัฐอเมริกา ได้ทำปฏิบัติการ “Operation Enduring Freedom” ในเดือนตุลาคม 2001 เพื่อโค่นล้มรัฐบาล Taliban โดยหลังการบุกครั้งแรก กลุ่ม Taliban ได้เริ่มทำสงครามกองโจรต่อสู้กับกองทัพสหรัฐฯ และหลังจากการเสียชีวิตของ บิน ลาเดนในปี 2011 สหรัฐฯ เริ่มถอนกำลังทหารออกไป เมื่อพิจารณาจากอัตราการเพิ่มขึ้นของอายุขัยต่อปีของช่วงเวลาสงคราม พบว่าอัตราการเพิ่มขึ้นของอายุขัยต่อปียังคงเพิ่มขึ้นเฉลี่ย 0.638%

**กราฟ 12 :** Afghanistan's Life Expectancy and Wars (2001–2014)
![image](https://github.com/user-attachments/assets/900aa4eb-58f2-43d6-9cd5-4b19791a5ab8)



## Question 4 : ปัจจัยอะไรบ้างที่ส่งผลต่อความสุข (Happiness)
จากการศึกษาความสัมพันธ์ (correlation) ของข้อมูลของ The World Happiness Report ในปี 2008 - 2023 พบว่า ปัจจัยที่สัมพันธ์กับความสุขมากที่สุด คือ ปัจจัยทางเศรษฐกิจ (GDP) อายุขัยเฉลี่ย (Life Expectancy) และการสนับสนุนทางสังคม (Social Support) ในขณะที่ค่าเฉลี่ยของการวัดผลอารมณ์ด้านลบ (Negative affect) และการรับรู้การคอร์รัปชัน (Corruption Perception) มีผลทำให้ความสุขลดลง ดังนั้นการลดปัจจัยเหล่านี้จะช่วยเพิ่มความสุขโดยรวมในสังคมได้ 
นอกจากนี้พบว่า การเอื้ออาทร ( Generosity ) ที่วัดจากการบริจาค ไม่ได้สัมพันธ์กับความสุขมากนัก

**กราฟ 13 :**  Correlation Between Factors and Happiness

![image](https://github.com/user-attachments/assets/ed4e649a-8001-4db3-b6fc-81ae2aa61348)

จากกราฟที่ 14 เกิดจากการนำข้อมูลของจาก Life Expectancy ของ WHO มา join กับ Happiness ก็จะมีสิ่งที่อธิบายได้เพิ่มขึ้น เช่น 
- ปัจจัยทางด้านเศรษฐกิจ (log GDP) มีความสัมพันธ์กันมากกับทั้งอายุขัยและความสุข (เมื่อ standardize กับ GDP อาจจะทำอธิบายได้ดีขึ้น)
- อายุขัยและความสุขมีความสัมพันธ์กันมากเป็นไปในทิศทางเดียวกัน
- การศึกษา (schooling) ก็สัมพันธ์กันค่อนข้างมากทั้งอายุขัยและความสุข
- ปัจจัยด้านการตายจะสัมพันธ์กันมากในทางตรงกันข้ามกับอายุขัย แต่กับความสุขจดลดความสัมพันธ์ลงมา 
- ปัจจัยด้านเสรีภาพ (Freedom) กับ Positive affect จะสัมพันธ์กับความสุขมากกว่าอายุขัย


**กราฟ 14 :**  Correlation Between Factors with Life Expectancy and Happiness
![image](https://github.com/user-attachments/assets/cb28c21f-f37e-4eab-a20e-cfe4a0b9a3d7)

## Question 5 : ประมาณการอายุขัยและความสุข มีความสัมพันธ์กันอย่างไร
จากกราฟพบว่า Life Expectancy กับ Happiness มีความสัมพันธ์ไปในทิศทางเดียวกัน กล่าวคือยิ่งอายุขัยมากจะยิ่งมีความสุขนั่นเอง

ทั้งนี้ได้ทางทีมได้จำลอง regression line ออกมาเป็น 3 เส้นที่ degree = 1,2,3 ตามลำดับ แต่ทำการวัดค่า MSE (Meas Square Error) ของแต่ละเส้นพบว่า ไม่ได้แตกต่างกันมาก และเนื่องจากอายุขัยของมนุษย์ แต่ทางทีมคิดว่าที่ degree = 2 หรือ 3 จะเหมาะสมกว่า
**กราฟ 15 :**  Life Expectancy and Happiness

![image](https://github.com/user-attachments/assets/1fd75012-f52d-4d43-9c8e-06149cc8ef42)


## Question ุ : นำข้อมูลมาใช้ประโยชน์กับประเทศไทยได้อย่างไรบ้าง
### 6.1 เปรียบเทียบจำนวนการเกิดและการตายของประชากรไทย
เมื่อนำข้อมูลจำนวนการเกิดและการตายที่ได้จาก ส่วนบริหารและพัฒนาเทคโนโลยีการทะเบียน มาเปรียบเทียบกันในช่วงปี 2002 - 2023 พบว่าในภาพรวมจำนวนการเกิดลดลงทุกๆปี ซึ่งสวนทางกับจำนวนการตายที่เพิ่มขึ้นทุกๆปี

โดยในปี 2012 จำนวนการเกิดทั้งเพศชายและหญิงมีแนวโน้มลดลงอยากเห็นชัดเมื่อเทียบกับช่วงเวลาก่อนหน้า  และสำหรับการตายที่ค่อยๆเพิ่มขึ้นได้ขยับสูงขึ้นอย่างชัดเจนในช่วงปี 2020 - 2022 ซึ่งเป็นช่วงเวลาเดียวกันกับเหตุการณ์ covid-19 

โดยในช่วงปี 2021 ประเทศไทยมีการตายมากกว่าการเกิดเป็นครั้งแรก จะทำให้จำนวนประชากรไทยเริ่มลดลงเรื่อย ๆ โดยเฉพาะเพศชายที่จำนวนการตายเฉลี่ยมากกว่าเพศหญิง ส่งผลกระทบทำให้ประชากรลดลง การเปลี่ยนแปลงในโครงสร้างประชากรและการเปลี่ยนแปลงทางสังคม

**กราฟ 16 :** เปรียบเทียบจำนวนการเกิดและการตายของประชากรไทย
![image](https://github.com/user-attachments/assets/269b4e8e-ef51-4682-8348-6c4d3ab16a52)

### 6.2 โครงสร้างประชากร
จากการเกิดที่ลดน้อยลง และอายุขัยที่ยาวขึ้น (2002 = 57.78 ปี, 2023 = 68.06 ปี) ทำให้ประชากรกลุ่มใหญ่ของประเทศ จากเดิมอยู่ในช่วงอายุ 20 - 39 ปี ในปี 2002 เป็นช่วงอายุ 40 - 59 ปี และอายุขัยของประชากรในช่วงอายุหลังจากนี้ก็ลดลงอย่างมีนัยสำคัญ 

- ประชากรวัยเด็กและเยาวชน(อายุไม่เกิน 20 ปี) ลดลงจากเดิม 19.40 ล้านคนในปี 2002 เหลือ 15.15 ล้านคนในปี 2023 (คิดเป็น 22.94 % ของประชากรรวมในปี 2023) 
- ประชากรวัยทำงาน (ตั้งแต่ 20 - 60 ปี) เพิ่มขึ้นเล็กน้อยจาก 37.07 ล้านคนในปี 2002 เป็น 38.61 ล้านคนในปี 2023 (คิดเป็น 58.44 % ของประชากรรวมในปี 2023) 
- ประชากรวัยเกษียณ (60 ปีขึ้นไป) เพิ่มขึ้นอย่าง 2.26 เท่า จากเดิม 5.43 ล้านคนในปี 2002 เป็น 12.30 ล้านคน ในปี 2023 (คิดเป็น 18.62 % ของประชากรรวมในปี 2023) 


**กราฟ 17 :** โครงสร้างประชากร
![image](https://github.com/user-attachments/assets/dec65cf1-bd6b-42de-8040-183eff99c52b)

![image](https://github.com/user-attachments/assets/4004fd59-fbfe-478d-92d3-2f1ffc4db01a)


### 6.3 งบประมาณ
จากข้อมูลงบประมาณย้อนหลังจาก สำนักงานพัฒนารัฐบาลดิจิทัล (องค์การมหาชน) (สพร.) พบว่า
-	โดยรวบงบปี 2024 เพิ่มขึ้นทั้งหมด โดยเฉพาะงบด้านสังคมสงเคราะห์กับด้านเศรษฐกิจที่เพิ่มค่อนข้างสูง 17-18% เมื่อเทียบกับปีก่อนหน้า
-	งบประมาณด้านเศรษฐกิจ เพิ่มขึ้นเกือบทุกปี และคิดเป็นประมาณ 20 – 25% ของงบประมาณทั้งหมด
-	งบด้านการศึกษาลดลงทุกปี โดยพึ่งจะเพิ่มขึ้นในงบประมาณปี 2024 เท่ากับ 0.76% และเมื่อเทียบสัดส่วนกับงบประมาณรวมจากเดิม ปี 2016 = 19.80 % เหลือ 12.64 % ในปี 2024
-	งบของกระทรวงสาธารณสุข จะค่อนข้างคงที่ คือโดยประมาณ 3 แสนล้านบาทแต่ในปี 2021 เพิ่มเป็น 3.43 แสนล้านบาท

**กราฟ 18 :** งบประมาณเปรียบเทียบ

![image](https://github.com/user-attachments/assets/ca54c03c-383e-498e-a884-fb7123803ef8)



จากกราฟที่ 19 พบว่า งบประมาณด้านเศรษฐกิจ ไม่ค่อยสัมพันธ์กันกับ GPD เห็นได้จาก ในปี 2016 ที่ใช้งบประมาณด้านเศรษฐกิจน้อยทุกปี แต่มี GPD ที่สูงกว่าปี 2019 เป็นต้นไปที่ใช้งบประมาณมากกว่า เป็นไปได้ว่างบประมาณที่ลงไปอาจจะไม่ทำให้เกิดการเติบโตทางเศรษฐกิจ หรือมีปัจจัยอื่นมากระทบ เช่น ปี 2020 แม้จะมีจัดสรรงบประมาณไปค่อนข้างเยอะ แต่พบว่า GDP ติดลบเนื่องจากภาวะโรคระบาด



**กราฟ 19 :** งบประมาณกับ GDP

![image](https://github.com/user-attachments/assets/21803a3f-45a8-4ee9-8036-59ea169c11e2)






## 6.4 บทสรุป
ในการวางแผนพัฒนาเศรษฐกิจของประเทศไทย ควรพิจารณาทั้งปัจจัยทางอายุขัยและโครงสร้างประชากรควบคู่กันไปด้วย นอกจากนี้ควรพิจารณาปัจจัยทางด้านความสุขประกอบกันด้วย
- การลดอัตราการตายลงทั้งในเด็กทารก เยาวชนและวัยผู้ใหญ่ ตลอดจนสร้างภูมิคุ้มกันในประชากร จะทำอายุขัยเฉลี่ยสูงขึ้น ซึ่งอาจจะต้องพิจารณางบด้านสาธารณะสุขให้เพิ่มขึ้น
- เนื่องด้วยแนวโน้มของอายุขัยเฉลี่ยที่เพิ่มขึ้น ประกอบกับโครงสร้างประชากรที่กำลังเปลี่ยนไป ประชากรกลุ่มผู้สูงอายุเพิ่มขึ้นในขณะที่ประชากรกลุ่มเด็กและเยาวชนลดลง อันเนื่องมาจากอัตราการเกิดที่ลดลง ควรเลื่อนอายุเกษียณเพื่อชะลอการขาดแคลนแรงงาน และลดภาระด้านงบประมาณด้านการสังคมสงเคราะห์
- และปัจจัยอายุขัยกับด้านเศรษฐกิจ (GDP)  มีความสัมพันธ์แบบส่งเสริมซึ่งกันและกัน กล่าวคือเมื่อประชากรอายุขัยเพิ่มขึ้นจะทำให้ค่า GDP เพิ่มขึ้นด้วย และเมื่อค่า GDP เพิ่มขึ้นกล่าวคือเศรษฐกิจโตขึ้น งบประมาณที่นำไปใช้เพื่อมีอายุขัยยืนยาวก็จะเพิ่มขึ้นด้วยเช่นกัน
- นอกจากนี้จำนวนชั่วโมงการเรียนก็มีผลอย่างมากทั้งด้านอายุขัยกับเศรษฐกิจ และจากอัตราการเกิดที่ลดลง ก็ควรพิจารณาโครงสร้างการศึกษาควบคู่กับงบประมาณ เช่น อาจจะเน้นในเชิงคุณภาพมากกว่าปริมาณ เป็นต้น
- และสุดท้ายทำให้ประชากรมีความสุข นอกเหนือจากการเพิ่มขึ้นของอายุขัย เศรษฐกิจ การศึกษาหรือปัจจัยสุขภาพแล้ว  ควรส่งเสริมให้มีการช่วยเหลือกันในสังคมและเสรีภาพในการเลือกใช้ชีวิต



