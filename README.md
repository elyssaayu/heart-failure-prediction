# 🫀 End-to-End Heart Failure Pipeline & Diagnostic Analysis

## 📌 Executive Summary
This project implements a complete data analysis pipeline analyzing cardiovascular disease indicators from 918 patient records from a Kaggle dataset. Using SQL, data ingestion, hypothesis testing and machine learning, the project identifies key physiological markers associated with heart failure and has built a predictive classification model with an 89% accuracy.

## 🛠️ Tech Stack & Methodology
* **Data Storage & Querying:** SQLite3, SQL
* **Data Wrangling & Cleaning:** Pandas, NumPy
* **Statistical Inference:** SciPy (`Two-Sample T-Test`)
* **Data Visualization:** Seaborn, Matplotlib
* **Machine Learning:** Scikit-Learn (`Random Forest`, ‘Local Outlier Factor’)

## 📊 Key Findings & Visualizations
1. **Statistical Significance:** A two-sample t-test revealed that patients with heart disease have a **statistically significant lower maximum heart rate (MaxHR)** ($p < 0.0001$) compared to healthy controls. Interestingly, Cholesterol and Resting Blood Pressure were found to have no statistically significant difference between heart disease patients and healthy controls.
2. **Predictive Modeling:** The Random Forest classification model achieved **~85% accuracy** in identifying heart disease risk based on routine clinical metrics.
3. **Feature Importance:** The Random Forest model also found that SlopeUp was the greatest classifier of heart disease, followed by MaxHR and OldPeak.

![MaxHR Distribution](output/maxhr_distribution.png)

## 🚀 How to Run
1. Clone repository: `git clone https://github.com/YOUR_USERNAME/heart-failure-pipeline.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Run the notebook in `src/pipeline.ipynb`

