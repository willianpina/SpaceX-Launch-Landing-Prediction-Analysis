# 🚀 SpaceX Launch Landing Prediction & Performance Analysis

## 📌 Project Overview

This project analyzes Falcon 9 launch records to understand landing success patterns and build predictive models capable of forecasting booster landing outcomes.

The analysis integrates:

* Exploratory Data Analysis (EDA)
* SQL-based data exploration
* Geospatial proximity analysis
* Interactive dashboard development (Plotly Dash)
* Machine Learning classification models

The goal is to combine **data analytics and predictive modeling** to extract operational insights from SpaceX launch data.

---

## 🎯 Objectives

* Identify which launch sites achieve the highest landing success rates
* Analyze the impact of payload mass on landing outcome
* Explore geographic proximity factors (coastline, infrastructure)
* Compare multiple classification algorithms
* Build an interactive dashboard for data-driven insights

---

## 📊 Exploratory Data Analysis

Key findings:

* Florida sites (KSC LC-39A and CCAFS LC-40) concentrate the majority of successful landings.
* Landing success significantly improved with newer booster versions (FT, B4, B5).
* Payload mass alone is not the primary determinant of failure.
* Higher success consistency observed in the 2000–5000 kg payload range.

---

## 🗺️ Geospatial Analysis

Using **Folium**, launch sites were mapped and analyzed for proximity to:

* Coastline
* Highways
* Railways

Key insight:

> Launch site positioning balances safety (over-water trajectories) with logistical efficiency.

---

## 📈 Interactive Dashboard (Plotly Dash)

The dashboard includes:

* Launch site filter (dropdown)
* Success vs failure pie charts
* Payload range slider
* Payload vs launch success scatter plot
* Booster version category visualization

This allows dynamic performance exploration across sites and payload ranges.

---

## 🤖 Machine Learning Models

Classification models implemented:

* Logistic Regression
* Support Vector Machine (SVM)
* Decision Tree
* K-Nearest Neighbors (KNN)

### 🏆 Best Performing Model

**Decision Tree**
Accuracy: **~88.6%**

---

## 📉 Confusion Matrix (Decision Tree)

|                | Predicted Fail | Predicted Success |
| -------------- | -------------- | ----------------- |
| Actual Fail    | 2              | 4                 |
| Actual Success | 2              | 10                |

### Model Behavior

* Strong detection of successful landings
* Slight tendency to overpredict success
* Balanced overall performance

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Plotly
* Dash
* Folium
* Scikit-learn
* SQL

---

## 📂 Project Structure

```
SpaceX-Launch-Landing-Prediction-Analysis/
│
├── data/
├── notebooks/
├── dashboard/
├── images/
├── maps/
└── README.md
```

---

## ▶️ Running the Project

Clone the repository:

```bash
git clone https://github.com/willianpina/SpaceX-Launch-Landing-Prediction-Analysis.git
cd SpaceX-Launch-Landing-Prediction-Analysis
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the dashboard:

```bash
python dashboard/app.py
```

---

## 📌 Business & Analytical Insights

* Booster evolution plays a larger role than payload mass in landing success.
* Florida is the operational core for Falcon 9 missions.
* Machine learning models can reliably predict landing outcomes.
* Operational maturity correlates with improved success consistency.

---

## 🔮 Future Improvements

* Add ensemble models (Random Forest, XGBoost)
* Perform k-fold cross-validation comparison
* Deploy dashboard to cloud
* Add real-time SpaceX API integration

---

## 👤 Author

**Willian Pina**
Data Scientist | Geospatial AI | Machine Learning

---
