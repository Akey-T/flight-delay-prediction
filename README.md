# Flight Delay Prediction

This project aims to predict whether a flight will be delayed using logistic regression.  
The dataset includes flight records with features such as date, time, airline, distance, and airport information.

---

## 1. Project Overview

The goal of this project is to build a classification model that predicts flight delays (1 = delayed, 0 = on-time).  
We use logistic regression as a baseline model and evaluate its performance using accuracy, precision, recall, and ROC-AUC score.

Main steps:
1. Data extraction and cleaning  
2. Feature engineering (date and time conversion, categorical encoding)  
3. Model training and testing  
4. Model evaluation (Confusion Matrix, ROC Curve)  
5. Deployment preparation on GitHub

---

## 2. Requirements

To run this notebook, install the required dependencies:

```bash
pip install -r requirements.txt
```

Key libraries used:
- pandas  
- numpy  
- scikit-learn  
- matplotlib  
- seaborn  
- jupyter

---

## 3. Files Description

```
flight-delay-prediction/
│
├── flight_delay.ipynb       # Main Jupyter Notebook containing data processing, model training, and evaluation
├── requirements.txt         # Python dependencies
├── README.md                # Project description
└── .gitignore               # (Optional) Ignore large files and data
```

---

## 4. How to Run

1. Open the notebook in Jupyter or VS Code:
   ```bash
   jupyter notebook flight_delay.ipynb
   ```
2. Run all cells sequentially.
3. The notebook will automatically:
   - Load and clean the flight data  
   - Train a logistic regression model  
   - Display confusion matrix and ROC curve  

---

## 5. Model Results Summary

**Model:** Logistic Regression  
**Test Accuracy:** ~0.58  
**Precision:** 0.27  
**Recall:** 0.57  
**Specificity:** 0.58  
**AUC:** 0.58  

**Confusion Matrix:**
|            | Predicted 0 | Predicted 1 |
|-------------|--------------|--------------|
| **Actual 0** | 150468       | 107984       |
| **Actual 1** | 29586        | 39080        |

Interpretation:
- The model performs moderately well in identifying on-time flights.  
- There is still room for improvement through feature engineering and model tuning.

---

## 6. Next Steps

- Test other classification algorithms (Random Forest, XGBoost, SVM).  
- Add weather and airport congestion data for better prediction accuracy.  
- Tune model hyperparameters using cross-validation.  

---

## 7. Author

**Author:** Akey-T  
**Repository:** https://github.com/Akey-T/flight-delay-prediction  
**Environment:** Python 3.11, Jupyter Notebook
