## Identifying Anomalies in Energy Sensor DataThis repository includes a machine learning project to identify anomalies from sensor data taken at an energy manufacturing facility. This project was done as part of a practical assessment in data science at Celebal Technologies. 

## Problem StatementGiven time-series sensor readings (X1 to X5) taken at equal time intervals; the goal is to identify anomalies where `target = 1` is an anomaly, and `0` is non-anomalous.

### Input Columns:
- Date: Timestamp (not used in model)- X1, X2, X3, X4, X5: Sensor readings
- target: Binary anomaly label (only used in training)

## Goals
- Data exploration, cleaning, and pre-processing
- Run various classical and advanced ML models
- Feature scaling, model tuning, and validation
- Model evaluation via Accuracy, F1 Score, etc.
- Make predictions and prepare for submission. 

## Files in this Repo

| File Name               | Description                           |
|-------------------------|---------------------------------------|
| train.csv               | Training dataset with labels          |
| test.csv                | Test dataset for prediction           |
| final_submission.csv    | Final output ready for submission     |
| Celebal-AnaVerse.ipynb  | Jupyter notebook with full workflow   |
| README.md               | Project overview and usage details    |

## Summary of Machine Learning Pipeline

### Preprocessing Data
- Removed the Date and ID column as not a feature column to analyze
- StandardScaler was used to scale the data.

### Creating a Model
- Started creating a lot of models before falling in creating a model on XGBoost.
- Created a train-test split of 80-20, stratified on target.

### Evaluation
- My evaluation metric were:
- Accuracy  
- F1 Score  
- Classification Report
- Strong performance when evaluated on validation set.

### Submission- Prediction in required format was saved in final_submission.csv

## Packages used- pandas, numpy- scikit-learn- xgboost- matplotlib, seaborn (optional for better visualization)

## How to Run

1. Clone this repo:

2. Open notebook.ipynb using Jupyter:

3. Install required libraries (if not already):

4. Run all cells and generate final_submission.csv

## Author

Rakesh Kumar Barik, Final Year B.E. CSE Student  
Aspiring Data Analyst | Python, SQL, Excel, Power BI  
LinkedIn: https://www.linkedin.com/in/rakeshbarik/

## Status

Project Completed  
Ready for deployment or extension (deep learning, time-series models, etc.)

