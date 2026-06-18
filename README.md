# House Price Prediction

**Author:** Eakansh Kshirsagar  
**Internship:** XYlofy (Week 1 Assignment)

## Overview
This project involves building a regression model to predict house prices based on property features such as area, number of bedrooms, bathrooms, and other amenities. 

## Tasks Completed (All 5 Required Tasks)
1. **Task 1 \u2014 Data Loading & Exploration:** Loaded the 545-row dataset and verified the structure and column types.
2. **Task 2 \u2014 Data Cleaning:** Confirmed there were no missing or duplicate values, and applied one-hot encoding to 7 categorical variables so the models could process them numerically.
3. **Task 3 \u2014 Model Building:** Trained, evaluated, and compared two algorithms: **Linear Regression** (MAE: 970,043, R\u00b2: 0.653) and **Random Forest Regressor** (MAE: 1,013,969, R\u00b2: 0.613).
4. **Task 4 \u2014 Visualization:** Created three required visualizations to analyze the data visually (price histogram, correlation heatmap, and actual vs. predicted prices).
5. **Task 5 \u2014 Insights & Summary:** Extracted feature importances to identify that **area** (46.9%) and **bathrooms** (15.3%) are the strongest predictors of house price, and provided a business recommendation.

## Files Included
- `analysis.ipynb`: The complete Jupyter Notebook containing all Python code, outputs, and the 5 completed tasks.
- `Housing.csv`: The original dataset used for training (545 rows, 13 columns).
- `summary.docx`: A concise 1-page business summary of the findings and model metrics.
- `charts/`: Folder containing all generated visualization PNGs.
