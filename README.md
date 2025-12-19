# Heart Failure Prediction Analysis

**Course:** INST447 - Data Analytics Team Project  
**Date:** Fall 2025  

## 👥 Team Members
* Joseph Choi
* Josue Aguilar
* Joshua Kwan
* Justin Monius

## 📌 Project Overview
This project analyzes clinical and demographic data to identify key risk factors associated with heart disease. Using the **Heart Failure Prediction Dataset**, our team performed data cleaning, exploratory data analysis (EDA), hypothesis testing, and predictive modeling to determine which variables—such as age, cholesterol, and exercise-induced angina—most strongly predict the presence of heart disease.

The final analysis includes significance testing (T-tests, Chi-Square) and a logistic regression model to inform potential healthcare screening strategies.

## 📂 Repository Structure
* **`heart_cleaned.csv`** - The processed dataset used for analysis (zeros in `RestingBP` and `Cholesterol` treated as NA).
* **`Heart_Failure_Analysis.Rmd`** (or `.R`) - The R source code containing data import, cleaning, visualizations, and statistical models.
* **`Project_Report.pdf`** - The final formal data analytics report (Deliverable 3).
* **`README.md`** - Project documentation.

## 📊 Dataset
**Source:** [Heart Failure Prediction Dataset (Kaggle)](https://www.kaggle.com/datasets/tan5577/heart-failure-dataset)  
**Description:** 918 observations with 12 attributes including:
* `Age`, `Sex`
* `ChestPainType`, `RestingBP`, `Cholesterol`
* `FastingBS`, `RestingECG`, `MaxHR`
* `ExerciseAngina`, `Oldpeak`, `ST_Slope`
* `HeartDisease` (Target: 1 = Disease, 0 = Normal)

## 🛠️ Technologies Used
* **Language:** R (v4.x)
* **IDE:** RStudio
* **Libraries:**
  * `ggplot2` (Visualization)
  * `dplyr` (Data Manipulation)
  * `skimr` (Data Summary)
  * `knitr` (Report Generation)

## 🔍 Key Findings
1.  **Max Heart Rate:** Patients with heart disease have significantly lower maximum heart rates ($M = 127.7$) compared to healthy patients ($M = 148.2$).
2.  **Exercise Angina:** This is a critical red flag. Patients experiencing chest pain during exercise are **over 2.5x more likely** to have heart disease.
3.  **Predictive Model:** Our logistic regression model confirmed that **Age**, **Sex (Male)**, **Exercise Angina**, and **Cholesterol** are all statistically significant predictors of heart failure ($p < .05$).

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone [https://github.com/Kwanjk/Heart-Failure-Dataset-.git](https://github.com/Kwanjk/Heart-Failure-Dataset-.git)

```

2. Open the project in **RStudio**.
3. Ensure the `heart.csv` (raw) or `heart_cleaned.csv` is in your working directory.
4. Install required packages:
```r
install.packages(c("ggplot2", "dplyr", "skimr", "knitr"))

```


5. Run the R script or Knit the RMarkdown file to generate the analysis and graphs.

---

*This project was completed for academic purposes at the University of Maryland.*
