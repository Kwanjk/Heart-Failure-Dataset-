# Heart Failure Prediction Analysis

**Course:** INST447 - Data Analytics Team Project  
**Date:** Fall 2025

## 👥 Team Members
- Joseph Choi
- Josue Aguilar
- Joshua Kwan
- Justin Monius

## 📌 Project Overview
This project analyzes clinical and demographic data to identify key risk factors associated with heart disease. Using the Heart Failure Prediction Dataset, our team performed data cleaning, exploratory data analysis, significance testing (t-tests, chi-square), and built a logistic regression model to identify predictors of heart disease and inform potential screening strategies.

## 📂 Repository Structure
- [**Team Project Report (Deliverable 3)**](https://docs.google.com/document/d/1Hfvrvvig_bbn6d-PCNxew0ZkcoJZrEbzsrQs87n6Zmw/edit?usp=sharing) — Full formal data analytics report and interpretation.
- `heart_cleaned.csv` — the processed dataset used for analysis (zeros in `RestingBP` and `Cholesterol` treated as NA).
- `Heart_Failure_Analysis.Rmd` (or `.R`) — R source containing data import, cleaning, visualizations, and statistical models.
- `Project_Report.pdf` — final formal data analytics report (Deliverable 3).
- `README.md` — project documentation.

## 📊 Dataset
**Source:** [Heart Failure Prediction Dataset (Kaggle)](https://www.kaggle.com/datasets/tan5577/heart-failure-dataset)  
**Description:** 918 observations with 12 attributes including:
- `Age`, `Sex`
- `ChestPainType`, `RestingBP`, `Cholesterol`
- `FastingBS`, `RestingECG`, `MaxHR`
- `ExerciseAngina`, `Oldpeak`, `ST_Slope`
- `HeartDisease` (Target: `1` = Disease, `0` = Normal)

## 🛠️ Technologies Used
- **Language:** R (v4.4.2)
- **IDE:** RStudio
- **Key libraries:**
  - `ggplot2` (visualization)
  - `dplyr` (data manipulation)
  - `skimr` (data summary)
  - `knitr` (report generation)

## 🔍 Key Findings
1. **Max Heart Rate:** Patients with heart disease have significantly lower maximum heart rates (M = 127.7) compared to healthy patients (M = 148.2).
2. **Exercise Angina:** Patients experiencing chest pain during exercise are over 2.5× more likely to have heart disease — a strong clinical indicator.
3. **Predictive Model:** A logistic regression model identified Age, Sex (Male), Exercise Angina, and Cholesterol as statistically significant predictors of heart disease in this dataset.

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/Kwanjk/Heart-Failure-Dataset-.git
   ```

2. Open the project in RStudio.
3. Make sure `heart.csv` (raw) or `heart_cleaned.csv` (processed) is in your working directory.
4. Install required packages (if not already installed):
   ```r
   install.packages(c("ggplot2", "dplyr", "skimr", "knitr"))
   ```

5. Open `Heart_Failure_Analysis.Rmd` and Knit the document, or run the R script to reproduce the analysis and figures.

---

This project was completed for academic purposes at the University of Maryland.
