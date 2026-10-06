# Stroke Prediction: Demographic vs Health Factors

**ML & AI Project – EL01 Group 5**

## About the Project

This project investigates whether **demographic data** or **health data** is a better predictor of stroke, and builds logistic regression models to predict stroke outcomes.

The problem is split into two parts:

- **Problem 1 – Demographic perspective:** gender, age, marital status, residence type
- **Problem 2 – Health perspective:** hypertension, heart disease, average glucose level, BMI, smoking status

### Approach

- Cleaned the data (removed ambiguous/missing values; no duplicate records)
- Exploratory analysis with correlation, histograms, violin plots, pair plots and heatmaps
- Handled the heavily imbalanced dataset (249 stroke vs 4,860 non-stroke cases) using **SMOTE** oversampling
- Built **logistic regression** models, since stroke is a binary outcome
- Evaluated with precision, recall, F1-score and accuracy, and compared each variable individually against stroke

## Team (3 members)

| Name |
|------|
| Tay Yuyang |
| Apichart Yapakdee |
| Wai Yan Myint |

## Dataset

The dataset is the **Stroke Prediction Dataset** from **Kaggle**, by fedesoriano:
https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset

It contains 5,110 patient records with 12 columns (id, gender, age, hypertension, heart_disease, ever_married, work_type, Residence_type, avg_glucose_level, bmi, smoking_status, stroke).

## Repository Contents

| File | Description |
|------|-------------|
| `ML_code.ipynb` | Jupyter notebook with the full analysis and models |
| `healthcare-dataset-stroke-data.csv` | Dataset (from Kaggle) |
| `Slides_Presentation.pptx` | Project presentation slides |

## How to Run

```bash
pip install numpy pandas seaborn matplotlib scikit-learn imbalanced-learn jupyter
jupyter notebook ML_code.ipynb
```

Keep the CSV in the same folder as the notebook.
