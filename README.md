# Employee Sentiment Analysis — Final LLM Assessment

**Author:** Darpan Naganpuriya  
**Email:** darpannaganpuriya@gmail.com  
**Project:** Final LLM Assessment — Employee Sentiment & Flight Risk Analysis  
**Repository:** https://github.com/darpannaganpuriya/Employee-Sentiment-Analysis  
 

---

## 🔍 Project Overview

This project performs **sentiment analysis on employee emails** to measure engagement, identify top positive/negative employees, detect flight risks, and predict future sentiment trends using Linear Regression.  
It includes six key tasks:
1. Sentiment Labeling  
2. Exploratory Data Analysis (EDA)  
3. Monthly Sentiment Scoring  
4. Employee Ranking  
5. Flight Risk Identification  
6. Predictive Modeling for Sentiment Trends  

---


## 🧠 Task Summary

### **1. Sentiment Labeling**
- Performed using **TextBlob** for polarity detection.  
- Polarity > 0 → **Positive**, Polarity < 0 → **Negative**, Polarity = 0 → **Neutral**.  
- A new column `Sentiment` was added to the dataset.  

### **2. Exploratory Data Analysis (EDA)**
- Checked for missing values and data types.  
- Found the majority of emails are neutral or positive.  
- Time-series plots revealed seasonal trends (spikes during Q2 months).  
- Visualized sentiment distribution using bar and pie charts.

### **3. Monthly Sentiment Scoring**
- Assigned scores: Positive = +1, Negative = -1, Neutral = 0.  
- Aggregated monthly sentiment scores per employee.  
- Scores reset each new month.

### **4. Employee Ranking**
- Ranked employees based on total monthly sentiment scores.  
- Extracted **Top 3 Positive** and **Top 3 Negative** employees per month.

### **5. Flight Risk Identification**
- Flagged employees with ≥ 4 negative messages within any rolling 30-day period.  
- These employees were added to the **Flight Risk List**.

### **6. Predictive Modeling**
- Built a **Linear Regression model** to predict monthly sentiment score trends.  
- Independent features:
  - Message frequency  
  - Average message length  
  - Word count per message  
- Evaluated model using **R²** and **MAE** metrics.  

---

## 🏆 Key Results & Summary

### **Top 3 Positive Employees**
1. **sally.beck@enron.com**  
2. **lydia.delgado@enron.com**  
3. **johnny.palmer@enron.com**

### **Top 3 Negative Employees**
1. **eric.bass@enron.com**  
2. **michael.holmes@enron.com**  
3. **melissa.barnes@enron.com**

### **Employees Flagged as Flight Risk**
- **eric.bass@enron.com**  
- **melissa.barnes@enron.com**

---

## 📊 Key Insights

1. Most employees show neutral or mildly positive communication tones.  
2. Sudden spikes in negative sentiment correlate with project deadlines.  
3. Employees flagged as flight risk exhibited consistent negativity before dropping communication volume.  
4. Average sentiment trends improve after HR engagement initiatives.  

