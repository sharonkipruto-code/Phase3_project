# Seasonal Flu Vaccine Prediction  
Phase 3 Classification Project

**Author:** Sharon Kipruto

---

## 📌 Project Overview

This project focuses on predicting whether an individual received a **seasonal flu vaccine** using demographic, health, behavioral, and belief-based survey data. The goal is to support **public health organizations** in identifying populations that may require targeted outreach to improve vaccination uptake.

This is a **binary classification problem**, where the target variable indicates whether a respondent received the seasonal flu vaccine.

---

## 🎯 Business Problem

Public health agencies face challenges in achieving high vaccination coverage due to varying beliefs, access, and behavioral factors. Accurately identifying individuals who are less likely to get vaccinated allows for:
- More effective public health messaging
- Targeted vaccination campaigns
- Better allocation of outreach resources

**Key Question:**  
Can we predict seasonal flu vaccine uptake based on an individual’s background, health status, beliefs, and behaviors?

---

## 👥 Stakeholder

- **Public Health Organizations**

---

## 📊 Dataset Description

The dataset comes from the **National 2009 H1N1 Flu Survey (NHFS)** and is hosted by DrivenData.

🔗 https://www.drivendata.org/competitions/66/flu-shot-learning/

### Target Variable
- **Seasonal Flu Vaccine** (Yes / No)

### Feature Categories
The dataset includes features grouped into the following categories:

- **Demographics:** age, gender, education, income, employment, household size  
- **Health Status:** general health, chronic conditions, insurance coverage  
- **Medical History:** prior vaccination behavior, healthcare usage  
- **Opinions & Beliefs:** perceived vaccine effectiveness, safety concerns, trust in healthcare  
- **Behavioral & Risk Factors:** exposure risk, social interaction patterns, preventive behaviors  

---

## 🧹 Data Preparation

The data preparation process included:
- Inspecting data structure and distributions
- Handling missing values using appropriate imputation strategies
- Encoding categorical variables
- Scaling numerical features where necessary
- Splitting data into training and testing sets

These steps ensured the data was clean, consistent, and ready for modeling.

---

## 🧠 Modeling Approach

This project evaluates multiple classification models, including:
- **Logistic Regression (Baseline Model)**
- Tree-based and ensemble models for performance improvement

A baseline model was first established to provide a performance benchmark. Additional models were then trained and tuned to improve predictive performance, particularly recall.

---

## 📈 Evaluation Metrics

The primary evaluation metric used in this project is:

- **Recall**

### Why Recall?
In a public health context, failing to identify individuals who are unlikely to get vaccinated (false negatives) can lead to missed intervention opportunities. Maximizing recall helps ensure that more at-risk individuals are correctly identified.

Additional metrics reported include:
- Accuracy
- Precision
- F1-score
- Confusion Matrix

---

## ✅ Final Model & Results

The final model was selected based on:
- Superior recall performance
- Balanced overall classification metrics
- Suitability for the public health use case

The results indicate that beliefs about vaccines, prior health behavior, and certain demographic factors play a significant role in vaccination decisions.

---

## 🚀 Recommendations

Based on the findings:
1. prioritize individuals with low predicted uptake.From the public sentiment we observe that 18-34 agegroup is the lowest point of engagement and vaccination rates, we need to raise this bar.
2. Target outreach campaigns
 since the model has high Recall(76%), use predicted probabilities to identify individuals with low likelihood of vaccination.
3. launch **severity awareness** campaigns-highlight statistics of people hospitalized by the flu each year. Focus on severity of the flu and risk perception(how easy it is to catch the flu) because the opinion_seas_vacc_effective is low and opinion_seas_risk is high since people are likely to get vaccinatyed if they feel the risk.
4. shift focus of campaigns from *where to get vaccine* to *why the flu is a serious risk* specifically targetting 18-24 and 65+ age groups.
5. social Media Engagements-Launch severity awareness campaigns on social media platforms to specifically reach the "younger" demographic (18–34), where public sentiment is currently lowest.
---

## ⚠️ Limitations & Future Work

**Limitations:**
- Survey-based data may include self-reporting bias
- The dataset reflects a specific time period and may not fully generalize to future populations

**Future Work:**
- Incorporate additional behavioral or geographic data
- Explore advanced ensemble or cost-sensitive models
- Evaluate model performance across different demographic subgroups

---


