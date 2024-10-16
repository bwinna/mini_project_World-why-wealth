
## Project : Life Expectancy Analysis
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


## Question 
ประมาณการอายุขัย (life expectancy) ของประชากรโลกเป็นอย่างไร

ปัจจัยอะไรบ้างที่ส่งผลต่อประมาณการอายุขัยเฉลี่ย และส่งผลอย่างไร

มีเหตุการณ์ใดบ้างที่อาจส่งผลต่อประมาณการอายุขัย

ปัจจัยอะไรบ้างที่ส่งผลต่อความสุข (Happiness)

ประมาณการอายุขัยและความสุข มีความสัมพันธ์กันหรือไม่ อย่างไร

นำข้อมูลมาใช้ประโยชน์กับประเทศไทยได้อย่างไรบ้าง



## Question 1: ประมาณการอายุขัยเฉลี่ย (Life Expectancy) ในปี 2000 - 2015 เป็นอย่างไร

### 1.1 ประมาณการอายุขัยเฉลี่ยทุกประเทศ

จากการ Research Data ที่ World Health Organization ได้เก็บรวบรวมประมาณการของอายุขัยเฉลี่ย (“อายุขัยฯ”) ของทุกประเทศตั้งแต่ปี 2000 ถึง 2015  พบว่ามีแนวโน้มค่อยๆ เพิ่มสูงขึ้น โดยในปี 2000 อายุขัยเฉลี่ยฯ เท่ากับ 66.4 ปี และค่อยๆ เพิ่มขึ้นเป็น 71.5 ปีในปี 2015 คิดเป็น 7.68% หรือ 0.57% ต่อปี  
นอกจากนี้พบว่า อัตราการเพิ่มขึ้นในปี 2006-2007 สูงกว่าปีอื่นๆ อยู่ที่ 1.04 - 1.17%

สำหรับประเทศไทยพบว่ามีอายุขัยเฉลี่ยฯ สูงกว่าค่าเฉลี่ยของทั้งโลก โดยมีอายุขัยเฉลี่ยในปี 2000 เท่ากับ 70.6 ปี และเพิ่มขึ้นเป็น 76.1 ปี ในปี 2015 คิดเป็น 7.79% หรือ 0.58% ต่อปี  
นอกจากนี้พบว่า อัตราการเพิ่มขึ้นในปี 2009 และปี 2011 สูงกว่าปีอื่นๆ อยู่ที่ 1.23% และ 1.08% ตามลำดับ

**กราฟ 1:** Life Expectancy Trendline of All Countries
![image](https://github.com/user-attachments/assets/8b39824c-04c7-48e0-9cc7-d6b3f62d0820)

### 1.2 ประมาณการอายุขัยของแต่ละทวีป

เมื่อเราแบ่งอายุขัยฯตามทวีป พบว่า ทุกทวีปมีแนวโน้มที่จะอายุขัยเพิ่มขึ้น โดย:

- **Africa** มีอัตราการเพิ่มขึ้นของอายุขัยสูงที่สุด โดยเพิ่มขึ้นจาก 54.1 ปีในปี 2000 เป็น 62.5 ปี ในปี 2015 หรือคิดเป็น 15.4%
- **Europe** และ **North America** มีอายุขัยฯเฉลี่ยสูงที่สุด แต่มีอัตราการเพิ่มขึ้นของอายุขัยต่ำกว่าเมื่อเทียบกับ **Asia** และ **Africa**

#### รายละเอียดเพิ่มเติม
- **Africa**: อายุขัยเฉลี่ยในแอฟริกาเพิ่มขึ้นจาก 54.1 ปี ในปี 2000 เป็น 62.5 ปี ในปี 2015 ซึ่งเพิ่มขึ้นถึง 8.4 ปี หรือคิดเป็น 15.4 % โดยเป็นทวีปที่มีอัตราการเพิ่มขึ้นสูงที่สุด
- **Asia**: อายุขัยเฉลี่ยเพิ่มขึ้นจาก 68.6 ปี ในปี 2000 เป็น 73.1 ปี ในปี 2015 ซึ่งเพิ่มขึ้น 4.5 ปี
- **Europe**: มีอายุขัยเฉลี่ยสูงที่สุดในทั้งปี 2000 และ 2015 โดยเพิ่มขึ้นจาก 74.8 ปี เป็น 78.4 ปี ซึ่งเพิ่มขึ้น 3.6 ปี
- **North and South America**: อายุขัยเฉลี่ยใกล้เคียงกัน ในปี 2000 คือ 71.6 ปี และ 70.8 ปี ตามลำดับ และในปี 2015 เป็น 74.5 ปี
- **Oceania**: อายุขัยเฉลี่ยเพิ่มขึ้นจาก 67.5 ปี ในปี 2000 เป็น 71.2 ปี ในปี 2015 ซึ่งเพิ่มขึ้น 3.7 ปี

**กราฟ 2:** Life Expectancy Trendline by Region
![image](https://github.com/user-attachments/assets/aa9d10e7-8c50-4345-9e03-7154ce03a967)
เมื่อพิจารณา **กราฟที่ 3** แสดงอายุขัยที่สูงที่สุด 5 อันดับในแต่ละทวีป จะเห็นได้ว่าทุกทวีปจะมีแนวโน้มที่อายุขัยเพิ่มขึ้น แต่ก็มีการกระจายที่แตกต่างกันออกไป เช่น:

- **Europe** จะมีอายุขัยเฉลี่ยสูงที่สุดและเส้นอายุขัยมีการกระจายตัวน้อย
- **North America** มีลักษณะการกระจายตัวคล้ายกับ Europe ยกเว้น **Canada** ที่มีอายุขัยสูงกว่าประเทศอื่นๆ
- **Asia** มีการกระจายตัวมากกว่า
- **Oceania** มีการแบ่งออกเป็น 2 กลุ่มชัดเจน
- **Africa** มีการเกาะกลุ่มกันแต่อายุขัยเฉลี่ยต่ำกว่าทวีปอื่นๆ

**กราฟ 3:** Top 5 Countries with the Highest Life Expectancy by Region
![image](https://github.com/user-attachments/assets/76330f19-e7bc-4152-9151-860b192c4f50)

### 1.3 ประมาณการอายุขัยของประเทศที่พัฒนาแล้วกับกำลังพัฒนา

จาก **กราฟที่ 4** และ **กราฟที่ 5** จะเห็นได้ว่า:


- กลุ่มประเทศที่พัฒนาแล้วมีอายุขัยเฉลี่ยสูงกว่ากลุ่มประเทศที่กำลังพัฒนาอย่างชัดเจน
- บางทวีปเช่น **Africa** และ **South America** มีเฉพาะประเทศที่กำลังพัฒนา ดังนั้นปัจจัยทางเศรษฐกิจก็อาจจะมีส่วนทำให้อายุขัยของประชากรเพิ่มขึ้น

**กราฟ 4:** Life Expectancy in Developed and Developing Countries by Region
![image](https://github.com/user-attachments/assets/2afc1a19-f98e-47d9-915b-6abb98d56c19)
**กราฟ 5:** Life Expectancy in Developed and Developing Countries
![image](https://github.com/user-attachments/assets/fcad2886-5dcf-4abc-9cb4-2f9fd11ac07f)

