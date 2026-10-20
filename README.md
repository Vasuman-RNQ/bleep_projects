# bleep_projects
Doing pre-internship projects



---
# Project 01 — Student Performance & Academic Analytics

## 1. Project Overview & Dataset

* **Dataset:** UCI Student Performance Dataset (Mathematics)


* **Problem Statement:** An educational institution wants to understand the factors associated with student academic performance.


* **Suggested Resume Title:** Student Performance & Academic Analytics using Python



---

## 2. Data Understanding & Setup

The project begins by importing necessary data science libraries (`pandas`, `numpy`, `matplotlib`, `seaborn`) and programmatically downloading the dataset from the UCI Machine Learning Repository.

* **Dataset Shape:** 395 rows, 33 columns


* **Target Variable:** `G3` (Final Grade, scored from 0 to 20)



---

## 3. Data Cleaning & Preprocessing

* **Missing Values & Duplicates:** Checked and verified zero missing values and zero duplicate records.


* **Feature Engineering:**
* `G_avg`: Average grade across periods G1, G2, and G3.


* `Pedu_total`: Combined parental education score (`Medu` + `Fedu`).


* `at_risk`: Binary indicator for students failing (`G3 < 10`).




* **Outlier Detection:** Used the Interquartile Range (IQR) method on student `absences`, detecting 15 outlier students with over 20 absences.



---

## 4. Exploratory Analysis & Key Insights

* **Final Grades Distribution:** The mean final grade (`G3`) across all students is approximately **10.42** out of 20.


* **Study Time Impact:** Students with higher weekly study times (`studytime` >= 5 hours) demonstrate higher mean final grades (11.40) compared to lower study tiers.


* **Gender Disparity:** Male students in this dataset show a slightly higher mean final grade (**10.91**) compared to female students (**9.97**).


* **Top Correlated Features with Final Grade (`G3`):**
* `G2` (Second Period Grade): $0.90$

* `G1` (First Period Grade): $0.80$

* `Medu` (Mother's Education): $0.22$

* `failures` (Past Class Failures): $-0.36$




---

## 5. Data Visualization Suite

A comprehensive suite of **17 visualizations** was generated and saved to the `plots/` directory, including:

1. **Histograms:** Distribution of final grades (`G3`), student age, and absences.


2. **Box Plots:** Final grades broken down by study time, address/family size, and gender.


3. **Bar Charts:** Impact of combined parental education, past failures, and travel time on final grades.


4. **Count Plots:** Extracurricular activities vs. at-risk status, and desire for higher education by gender.


5. **Scatter Plots:** Absences vs. final grades, and Period 1 grade (`G1`) vs. Final grade (`G3`).


6. **Correlation Heatmap:** Full feature correlation matrix.


7. **Progression Chart:** Average student grade trend across academic periods (`G1` $\rightarrow$ `G2` $\rightarrow$ `G3`).


8. **Additional Analyses:** Violin plots for health status and overall student performance tier breakdown.


# Project 02 — Employee Attrition & Workplace Analytics

## 1. Project Overview & Dataset

* **Dataset:** IBM HR Analytics Employee Attrition & Performance Dataset
* **Problem Statement:** Understand the primary drivers behind employee turnover and identify patterns associated with high-risk attrition.
* **Suggested Resume Title:** Employee Attrition & Workforce Analytics using Python

---

## 2. Data Understanding & Setup

The project begins by importing necessary data science libraries (`pandas`, `numpy`, `matplotlib`, `seaborn`), setting visual themes, and inspecting dataset shapes, columns, and data types to establish a solid foundation for analysis.

---

## 3. Data Cleaning & Preprocessing

* **Data Quality Checks:** Handling missing values, checking for duplicate rows, and verifying data integrity.
* **Type Correction & Filtering:** Correcting data types and filtering datasets to prepare relevant employee features for subsequent exploratory and predictive analysis.

---

## 4. Exploratory Analysis & Key Insights

* **Univariate & Bivariate Analysis:** Examining individual workforce distributions and relationships between demographic/job-related features.
* **Multivariate & Correlation Analysis:** Utilizing correlation matrices to study statistical dependencies between key metrics such as Monthly Income, Job Satisfaction, OverTime, and overall attrition risk.

---

## 5. Data Visualization Suite

A comprehensive suite of charts and visualizations was generated to fulfill exploratory requirements:

1. **Histograms:** Distribution analysis of numerical features (e.g., Age, Monthly Income, Years at Company).
2. **Box Plots:** Outlier detection and evaluation across different job roles and departments.
3. **Bar Charts & Count Plots:** Ranking top categories and categorical trends (e.g., OverTime, Department, Business Travel).
4. **Scatter Plots:** Multi-variable relationship tracking between tenure, compensation, and performance metrics.
5. **Correlation Heatmaps:** Visualizing statistical dependencies across all numerical workforce features.
6. **Trend & Metric Tracking:** Monitoring workforce dynamics and key performance indicators.
