# 🫀 End-to-End Heart Failure Pipeline & Diagnostic Analysis

## 📌 Executive Summary
This project implements a complete data analysis pipeline analyzing cardiovascular disease indicators from 918 patient records from a [Kaggle](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction) dataset. Using SQL, data ingestion, hypothesis testing and machine learning, the project identifies key physiological markers associated with heart failure and has built a predictive Random Forest classification model with an 91% accuracy.

## 🛠️ Tech Stack & Methodology
* **Data Storage & Querying:** SQLite3, SQL
* **Data Wrangling & Cleaning:** Pandas, NumPy
* **Statistical Inference:** SciPy (`Two-Sample T-Test`)
* **Data Visualization:** Seaborn, Matplotlib
* **Machine Learning:** Scikit-Learn (`Random Forest`, 'Logistic Regression', ‘Local Outlier Factor’)

## 📊 Key Findings & Visualizations
1. **Statistical Significance:** A two-sample t-test revealed that patients with heart disease have a **statistically significant lower maximum heart rate (MaxHR)** ($p < 0.005$) compared to healthy controls.
2. **Predictive Modeling:** The Random Forest classification model achieved **~91% accuracy** in identifying heart disease risk based on routine clinical metrics.
<img width="775" height="640" alt="confusion matrix" src="https://github.com/user-attachments/assets/74247c44-2917-4630-96db-91d7cee0eed6" />

3. **Feature Importance:** The Random Forest model also found that SlopeUp was the greatest classifier of heart disease, followed by MaxHR and OldPeak.
 <img width="1060" height="580" alt="feature importance" src="https://github.com/user-attachments/assets/3257723a-a981-4d06-b9b2-1db58760a230" />

4. **Diagnostic Concordance:** The Local Outlier Factor model found that **~74% of anomalous profiles** belonged to heart disease patients, showing that physical extremity strongly correlates with actual cardiac pathology.



📄 Download or view the detailed data analysis pipeline in [Heart Failure Prediction Report](Heart%20Failure%20Prediction%20Report.pdf)

## 🚀 How to Run
1. Clone repository: `git clone https://github.com/elyssaayu/heart-failure-prediction.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Run the notebook in `src/Heart_Failure_Prediction.ipynb`

