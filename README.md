# 📊 Bellabeat Case Study using Microsoft Excel, SQL, and Power BI  
**How Can a Wellness Technology Company Play It Smart?**  

![Bellabeat logo](https://github.com/user-attachments/assets/8b00a978-b3f7-4685-8f19-29c80277a9e3)  

## 📌 Introduction  
In this case study, I analyze historical smart device usage data from **Bellabeat**, a high-tech wellness company specializing in health-focused products for women.  

### 🔍 **Objective**  
The goal is to identify **key trends in consumer behavior** and provide **data-driven recommendations** to optimize Bellabeat’s marketing strategy.  
To answer the key business questions, I follow the **Google Data Analytics** process:  
**Ask → Prepare → Process → Analyze → Share → Act**.  

### 🛠 **Tools Used**  
- **Microsoft Excel** – Merging tables for easy data handling  
- **SQL (MySQL)** – Data cleaning and processing  
- **Power BI** – Data visualization  

---

## 🔹 Quick Links  

📂 **Data Source**: [Fitbit Smart Device Dataset](https://www.kaggle.com/datasets/arashnic/fitbit)  

📝 **SQL Queries**: [Data Cleaning and Manipulation](https://github.com/nazim800/Bellabeat-Case-Study/blob/main/Data%20Cleaning%20and%20Manipulation)  

📊 **Data Visualizations**: [Power BI Report](https://github.com/nazim800/Bellabeat-Case-Study/blob/main/Bellabeat%20Final%20Visualization.pdf)  

📄 **Detailed Case Study Report**: [View PDF](https://github.com/nazim800/Bellabeat-Case-Study/raw/main/BellaBeat%20Case%20Study%20Report.pdf)  

---


## **Scenario**
As a **junior data analyst** on the **Bellabeat marketing analytics team**, I have been tasked with analyzing smart device usage data to uncover key trends and insights. Our team is responsible for collecting, analyzing, and reporting on consumer behavior to guide Bellabeat’s marketing strategy.

**Objective:**
- Analyze smart device usage data to identify consumer trends.
- Compare patterns in activity, sleep, stress, and hydration tracking.
- Discover how Bellabeat’s marketing team can leverage these insights.
- Present high-level recommendations to the Bellabeat executive team.

By the end of this analysis, Bellabeat will have **actionable insights** that can shape its marketing strategy and support its continued growth in the wellness technology market.

---
## **📌 Background**

**About Bellabeat:**
- A high-tech wellness company focused on **women’s health**.
- Founded in **2013** by **Urška Sršen** and **Sando Mur**.
- Offers smart wellness products such as:
  - **Leaf** (Wellness Tracker)
  - **Time** (Smartwatch)
  - **Spring** (Smart Water Bottle)
- **Connected to the Bellabeat app** for activity, sleep, stress, hydration, and mindfulness insights.

### **🔹 Business Growth Strategy**
Bellabeat aims to expand further and become a global leader in smart devices. To achieve this, it invests heavily in **digital marketing** via:
- **Google Search**
- **Facebook & Instagram**
- **YouTube**
- **Google Display Network**

Bellabeat’s leadership believes that **data-driven marketing** could unlock new growth opportunities.

---
## **Phase 1️⃣: Ask – Define the Business Problem**

### **🎯 Business Task:**
Bellabeat wants to use **smart device data** to gain insights into how customers interact with their products and identify opportunities for growth. The marketing team needs **data-driven recommendations** to refine their strategy and attract more customers.

### **🔑 Key Questions:**
1. What are the **current trends** in smart device usage?
2. How can these **trends apply** to Bellabeat customers?
3. How can these insights **shape Bellabeat’s marketing strategy**?

### **👥 Stakeholders:**
- **Urška Sršen** (Co-founder & Chief Creative Officer) – Seeks data-driven insights to inform business strategy.
- **Bellabeat Marketing Team** – Uses insights to optimize digital marketing campaigns.
- **Bellabeat Executive Team** – Requires recommendations for expanding market presence.

---
## **Phase 2️⃣: Prepare – Understanding and Preparing the Data**

### **📂 Data Source:**
- Dataset: **FitBit Fitness Tracker Data** (Kaggle, **CC0 Public Domain license**).
- Includes **daily activity levels, step counts, heart rate monitoring, and sleep patterns**.

### **📊 Data Organization & Storage:**
- Multiple **CSV files** representing different fitness tracking metrics.
- **Wide format**: Each row represents a single day’s activity for a user.
- Data was **imported into SQL for cleaning and analysis**.
- **Power BI used for visualization**.

### **⚠ Data Credibility & Limitations:**
- Limited to **30 users** (small sample size, may not represent broader trends).
- Potential **bias**, as data includes only users who consented to share.
- Lacks **demographics** (age, gender, location), making segmentation difficult.

### **✔ Addressing Data Integrity & Limitations:**
- Verified **data quality** (checked for missing values, duplicates, inconsistencies).
- **Filtered incomplete records** to ensure accuracy.
- Considered the need for **additional datasets** to supplement demographic insights.

---
## **Phase 3️⃣: Process – Cleaning and Preparing Data for Analysis**

### **🛠 Tools Used:**
- **Microsoft Excel** – Initial merging of tables.
- **MySQL** – Data cleaning & transformation.
- **Power BI** – Analysis & visualization.

### **🔍 Data Cleaning & Manipulation Steps in MySQL:**
#### **1. Check for Missing Values and Handle Them**
- Used SQL queries to **identify missing values**.
- Replaced missing data with **average/median values** (if possible).
- Removed records with **excessive missing fields**.

#### **2. Remove Duplicates**
- Identified duplicate records using SQL.
- Removed duplicates to ensure accurate analysis.

✔ **Summary of Data Cleaning Process:**
- Checked for **missing values** & handled them.
- Removed **duplicate records**.

---
## **Phase 4️⃣ & 5️⃣: Analyze Trends & Share Visualizations**

### **📊 Key Smart Device Usage Trends**

#### **📍 Trend 1: Users Are Most Active in the Morning & Evening**
- **Peak activity**: **7-9 AM** & **6-9 PM**.
- **Afternoon dip**: Users are less active during working hours.

✅ **Insights:**
- Send **weekend workout reminders** to boost engagement.
- **Target morning fitness campaigns** (since workouts are popular in the morning).

#### **📍 Trend 2: Higher Activity Leads to Better Sleep**
- Users **with more than 5,000 steps/day** have better sleep patterns.
- **Low activity (<5,000 steps/day) = inconsistent sleep**.

✅ **Insights:**
- Market Bellabeat devices as **sleep improvement tools**.
- Send **evening walk reminders** for better sleep.

#### **📍 Trend 3: High Heart Rate Correlates with Intense Activity Periods**
- **Morning & evening heart rate spikes** confirm **workout engagement**.

✅ **Insights:**
- Promote **early morning fitness challenges**.
- Add **heart rate tracking reminders** in fitness plans.

#### **📍 Trend 4: Weight Tracking Behavior Varies Among Users**
- Users who **manually track weight** have **lower BMI** & are **more engaged**.

✅ **Insights:**
- Encourage **manual weight logging**.
- Use **push notifications & gamification** (badges, streaks) to improve engagement.

---
## **Phase 6️⃣: Act – Recommendations**

### **📌 1. Promote Bellabeat as a Sleep & Wellness Solution**
- Emphasize **activity → better sleep connection** in marketing.
- Use **push notifications & emails** for sleep improvement tips.

### **📌 2. Introduce Smart Workout & Sleep Reminders**
- Send **morning workout notifications (6-9 AM)**.
- Launch **fitness challenges** during peak engagement hours.

### **📌 3. Encourage Weight & BMI Tracking**
- Promote **manual weight logging**.
- Add **badges & streaks** to encourage tracking.

### **📌 4. Develop Personalized Health Insights**
- Implement **AI-driven recommendations** in the Bellabeat app.
- Offer **weekly reports & adaptive challenges**.

---
🚀 **Conclusion:**
By leveraging **smart device data insights**, Bellabeat can improve **marketing strategies**, increase **user engagement**, and solidify its **position in the wellness technology market**.



