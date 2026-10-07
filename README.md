# 🏥 Hospital Readmission Risk Analysis

## 📝 Short Description
An Excel and Power BI project that analyzes 18,000 patient records to find which patients are most likely to be readmitted within 30 days of discharge. It builds a simple, explainable Low / Medium / High risk score so a hospital can decide who to flag for intensive follow-up after discharge.

## 🛠️ Tech Stack
  📗 **Microsoft Excel** - Data cleaning, helper columns , PivotTables, formula-driven risk scoring, High-risk action list 
  
  🧠 **DAX** - 7 measures for patient counts, readmission rate, gap vs overall and high-risk share 
  
  📊 **Power BI** - Data modelling

## 📂 Data Source
  🔗 Hospital Readmission Risk dataset from Kaggle
  https://www.kaggle.com/datasets/sunil123kumar/hospital-readmission-risk-dataset-csv
  
## ✨ Highlights

### ❗ Business Problem
Hospitals are measured on how many patients return within 30 days of discharge. A readmission often signals incomplete care, costs the hospital money and is hard on the patient. A hospital cannot give intensive follow-up (calls, early appointments, home visits) to every patient, so it needs to know who is most at risk.

**❓ Question answered:** *Which patient profiles have the highest 30-day readmission risk, and who should the hospital flag for intensive follow-up after discharge?*

### 🎯 Goal of the Dashboard
1. 📏 Show how big the readmission problem is.
2. 👥 Show which patient groups are readmitted more often.
3. 🔍 Identify the factors that go with higher risk.
4. 🚩 Combine those factors into a risk score and list the patients to flag.

### 🖼️ Walkthrough of Key Visuals

**📌 Page 1: Overview**
KPI cards (total patients, readmitted patients, readmission rate, high-risk share) and readmission rate by primary diagnosis.

**👤 Page 2: Patient Profile**
Readmission rate by age group, gender, insurance type, admission type, length of stay and discharge type.

**📈 Page 3: Risk Drivers**
Readmission rate by severity, number of medications, previous admissions, previous readmissions, chronic conditions, comorbidity index and high-risk medication use.

**🚨 Page 4: Risk and Action**
Readmission rate and patient count for each risk band, plus the high-risk share by age group.

### 💡 Business Insights

**🔑 Key findings**
  📊 The overall 30-day readmission rate is **74.2%** (13,349 of 18,000 patients).
  
  ✅ **Risk score works:** readmission rate rises from **68.1%** (Low) to **74.8%** (Medium) to **81.1%** (High), a gap of about 13 points between Low and High.
  
  🚩 **3,200 patients (17.8%)** fall in the High band and are the suggested group for intensive follow-up.
  
  👴 **Age 81 and over** stands out: **38.2%** of these patients are High risk versus about 15% in other age groups.


**✅ Recommendation**
Flag the High-risk patients for intensive follow-up after discharge, starting with those who have the highest scores and patients aged 81 and over. The full High-risk patient list is in the `Action_List` sheet of the Excel workbook.
