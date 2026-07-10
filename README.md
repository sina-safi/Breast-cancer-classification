# Breast Cancer Classification using Machine Learning

## Overview

This project applies machine learning techniques to classify breast cancer tumors as **benign** or **malignant** using the Wisconsin Breast Cancer Dataset.

The project covers the complete machine learning workflow, including data preprocessing, exploratory data analysis (EDA), feature scaling, hyperparameter tuning, model comparison, and performance evaluation.

---

## Project Preview

### ROC Curve

![ROC Curve](images/roc_curve.png)

### Confusion Matrix

![Confusion Matrix](images/confusion_matrix.png)

---

## Dataset

- **Dataset:** Wisconsin Breast Cancer Dataset
- **Source:** UCI Machine Learning Repository
- **Samples:** 569
- **Features:** 30 numerical features
- **Target:** Diagnosis (Benign / Malignant)

---

## Project Workflow

- Data cleaning
- Exploratory Data Analysis (EDA)
- Correlation analysis
- Train / Validation / Test split (70% / 15% / 15%)
- Outlier handling using a custom Winsorizer
- Feature scaling with MinMaxScaler
- Model training
- Hyperparameter tuning using GridSearchCV
- Model evaluation
- ROC Curve and Confusion Matrix visualization

---

## Machine Learning Models

The following classification algorithms were evaluated:

- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- Gaussian Naive Bayes

---

## Results

| Metric | Score |
|--------|------:|
| Accuracy | **97%** |
| Precision | **97%** |
| Recall | **94%** |
| F1-score | **95%** |
| ROC-AUC | **0.998** |

Among the evaluated models, **Logistic Regression** achieved the best overall performance on the test set.

---

## Technologies

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

---

## Repository Structure

```text
Breast-cancer-classification/
│
├── README.md
├── requirements.txt
├── Breast-cancer-classification.ipynb
└── images/
    ├── correlation_heatmap.png
    ├── confusion_matrix.png
    ├── model_accuracy.png
    └── roc_curve.png
```

---

## Installation

```bash
git clone https://github.com/sina-safi/Breast-cancer-classification.git

cd Breast-cancer-classification

pip install -r requirements.txt
```

---

## Running the Project

Open the Jupyter Notebook:

```bash
jupyter notebook Breast-cancer-classification.ipynb
```

or open it directly in **Google Colab**.

---

## Future Improvements

Possible extensions of this project include:

- Feature selection techniques
- XGBoost and LightGBM models
- Explainable AI using SHAP
- Model deployment with Streamlit

---

## Disclaimer

This project was developed for educational and portfolio purposes only. It should **not** be used for medical diagnosis or clinical decision-making.

---

## Author

**Sina Safi**

GitHub: https://github.com/sina-safi