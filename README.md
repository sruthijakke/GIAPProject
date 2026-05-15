# Diabetes Prediction Using Machine Learning

A capstone project that uses the PIMA Indians Diabetes Dataset from Kaggle to build and compare machine learning models for predicting diabetes.

---

## Dataset

**Name:** PIMA Indians Diabetes Database  
**Source:** [Kaggle](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)  
**File:** `diabetes.csv`  
**Rows:** 768 | **Features:** 8 | **Target:** `Outcome` (0 = No Diabetes, 1 = Diabetes)

---

## Project Structure

```
diabetes-prediction/
│
├── diabetes_prediction.py   # Main ML script
├── diabetes.csv             # Dataset (download from Kaggle)
├── requirements.txt         # Python dependencies
├── README.md                # This file
│
└── outputs/                 # Generated after running the script
    ├── correlation_heatmap.png
    ├── outcome_distribution.png
    ├── feature_distributions.png
    ├── confusion_matrices.png
    ├── roc_curves.png
    └── feature_importance.png
```

---

## Models Used

| Model | Description |
|---|---|
| Logistic Regression | Simple, interpretable baseline |
| Decision Tree | Rule-based classifier (max_depth=5) |
| Random Forest | Ensemble of 100 decision trees |

---

## How to Run

**1. Clone the repository**
```bash
git clone https://github.com/sruthijakke/giap project.git
cd diabetes-prediction
```

**2. Install dependencies**
```bash
pip install -r requirements.txt
```

**3. Download the dataset**

Go to [Kaggle](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database), download `diabetes.csv`, and place it in the project root folder.

**4. Run the script**
```bash
python diabetes_prediction.py
```

All charts will be saved as `.png` files in the same directory. Results will be printed in the terminal.

---

## Results (Sample)

| Model | Accuracy | ROC-AUC | CV Accuracy |
|---|---|---|---|
| Logistic Regression | ~77% | ~0.83 | ~77% |
| Decision Tree | ~75% | ~0.78 | ~75% |
| Random Forest | ~78% | ~0.84 | ~77% |

> Exact values may vary slightly depending on the environment.

---

## Requirements

- Python 3.8+
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

---
