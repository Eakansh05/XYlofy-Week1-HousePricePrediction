# 🏡 House Price Prediction Regression Analysis

[![Python 3.14](https://img.shields.io/badge/Python-3.14-blue.svg)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-0.24+-orange.svg)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/pandas-Data_Analysis-150458.svg)](https://pandas.pydata.org/)

**Author:** Eakansh Kshirsagar  
**Project Type:** XYlofy Internship \u2014 Week 1 Assignment

---

## 📖 Overview

This repository contains a complete end-to-end Machine Learning pipeline designed to predict housing prices based on property features. The project demonstrates proficiency in data wrangling, feature engineering, statistical analysis, and predictive modeling using standard Python data science libraries.

By comparing a **Linear Regression** baseline against a more complex **Random Forest Regressor**, this analysis identifies the most significant drivers of real estate pricing to provide actionable business recommendations.

---

## 🗂️ Dataset Details

- **File:** `Housing.csv`
- **Dimensions:** 545 rows \u00d7 13 columns
- **Target Variable:** `price` (Continuous)
- **Features Included:** Area, Bedrooms, Bathrooms, Stories, Mainroad, Guestroom, Basement, Hotwaterheating, Airconditioning, Parking, Prefarea, Furnishingstatus.

---

## ⚙\ufe0f Methodology (The 5 Required Tasks)

This project strictly follows the 5-step data science lifecycle outlined in the assignment requirements:

1. **Task 1 \u2014 Data Loading & Exploration:** 
   - Loaded the raw dataset and performed initial Exploratory Data Analysis (EDA).
   - Verified data integrity and column distributions.
2. **Task 2 \u2014 Data Cleaning:** 
   - Verified absence of missing values and duplicate rows.
   - Applied **One-Hot Encoding** (`get_dummies`) to 7 categorical variables.
   - Standardized boolean fields into integer formats for algorithmic compatibility.
3. **Task 3 \u2014 Model Building:** 
   - Split data into Training (80%) and Test (20%) sets.
   - Trained a **Linear Regression** model.
   - Trained a **Random Forest Regressor** (n_estimators=200).
4. **Task 4 \u2014 Data Visualization:** 
   - Plotted a price distribution histogram.
   - Generated a feature correlation heatmap.
   - Created an Actual vs. Predicted scatter plot for the Random Forest model.
5. **Task 5 \u2014 Insights & Summary:** 
   - Extracted feature importances to determine the strongest price predictors.
   - Summarized metrics (MAE, RMSE, R\u00b2) to evaluate model efficacy.

---

## 📊 Key Findings & Results

### Model Performance
| Model | Mean Absolute Error (MAE) | R\u00b2 Score |
|-------|--------------------------|----------|
| **Linear Regression** | `970,043` | `0.653` |
| **Random Forest** | `1,013,969` | `0.613` |

*Both models explain roughly 61-65% of the variance in house prices, providing a solid baseline for price estimation.*

### Top 3 Price Drivers (Feature Importance)
1. **Area (46.9%)** \u2014 The raw square footage dominates the pricing model.
2. **Bathrooms (15.3%)** \u2014 More impactful than the number of bedrooms.
3. **Air Conditioning (6.0%)** \u2014 The single most valuable non-structural amenity.

---

## 💻 How to Run Locally

If you wish to run the analysis on your local machine, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Eakansh05/XYlofy-Week1-HousePricePrediction.git
   cd XYlofy-Week1-HousePricePrediction
   ```

2. **Install the required dependencies:**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

3. **Launch the Jupyter Notebook:**
   ```bash
   jupyter notebook analysis.ipynb
   ```

---

## 📁 Repository Structure

```text
\u251c\u2500\u2500 charts/                     # Generated visual outputs
\u2502   \u251c\u2500\u2500 actual_vs_predicted.png
\u2502   \u251c\u2500\u2500 correlation_heatmap.png
\u2502   \u2514\u2500\u2500 price_histogram.png
\u251c\u2500\u2500 Housing.csv                 # Raw dataset
\u251c\u2500\u2500 README.md                   # Project documentation
\u251c\u2500\u2500 analysis.ipynb              # Main Jupyter Notebook
\u2514\u2500\u2500 summary.docx                # 1-page business report
```
