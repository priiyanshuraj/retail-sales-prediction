# 🛒 Online Shoppers Purchase Intention Prediction

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Classification-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Project Overview
This repository contains an academic machine learning project focused on predicting whether an online shopper will make a purchase (**Revenue = True/False**) based on their browsing behavior.

The project applies data preprocessing, exploratory data analysis (EDA), and multiple classification models, followed by a comparative performance evaluation to determine the most effective algorithm.

---

## 🎯 Project Objectives
- To analyze real-world e-commerce user behavior data.
- To preprocess and clean a structured retail dataset.
- To implement multiple machine learning classification models.
- To compare models using standard evaluation metrics.
- To identify the best-performing model for purchase prediction.

---

## 📊 Dataset Description
**Dataset:** Online Shoppers Intention Dataset  
**Source:** Kaggle  
**Total Records:** ~12,000 user sessions  

**Target Variable:** `Revenue`
- `True` → Purchase made
- `False` → No purchase

**Key Features:**
- **Page visit counts:** Administrative, Informational, ProductRelated
- **Duration:** Time spent on each page category
- **Metrics:** Bounce Rate, Exit Rate
- **Demographics/Context:** Browser, Region, Traffic Type, Weekend indicator

---

## 🧹 Data Preprocessing
The following steps were performed to ensure data quality and model reliability:
1. **Cleaning:** Removal of duplicate entries.
2. **Validation:** Checking for and handling missing values.
3. **Transformation:** Conversion of integer-coded categorical features into proper categorical types.
4. **Inspection:** Dataset analysis using `.info()` and `.describe()`.
5. **Splitting:** Train–test split to ensure unbiased evaluation.

---

## 🧠 Machine Learning Models Implemented
The project focuses on the following classification algorithms:

1. **Logistic Regression:** Used as a baseline model.
2. **Decision Tree Classifier:** To capture non-linear patterns.
3. **Random Forest Classifier:** An ensemble method to reduce overfitting and improve accuracy.

*All models were trained and tested using the same dataset split to ensure a fair comparison.*

---

## 📈 Evaluation Metrics
The models were evaluated using the following metrics:

- **Accuracy:** Percentage of total predictions that were correct.
- **Precision:** Out of all predicted purchases, how many were actually purchases.
- **Recall:** Out of all actual purchases, how many were correctly identified.
- **F1-Score:** Harmonic mean of Precision and Recall (useful for imbalanced classes).
- **Confusion Matrix:** visualizes correct and incorrect predictions across both classes.

---

## 📊 Model Performance Results

### 🔢 Classification Report Summary

| Model | Accuracy | Precision | Recall | F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| **Logistic Regression** | 0.84 | 0.79 | 0.56 | 0.65 |
| **Decision Tree** | 0.86 | 0.73 | 0.68 | 0.70 |
| **Random Forest** | **0.90** | **0.84** | **0.71** | **0.77** |

### 📌 Interpretation of Results

1.  **Logistic Regression**
    * Performs well as a baseline model.
    * High interpretability but lower recall indicates missed purchase opportunities.

2.  **Decision Tree**
    * Captures non-linear patterns better than Logistic Regression.
    * Improved recall but showed signs of overfitting.

3.  **Random Forest (🏆 Best Model)**
    * Achieved the highest Accuracy (90%) and F1-score.
    * Provided the best balance between precision and recall.
    * Reduced overfitting due to the nature of ensemble learning.

---

## 🏆 Final Conclusion
✅ **Random Forest Classifier is the best-performing model for this dataset.**

This project confirms that:
* Ensemble methods outperform single estimators in complex classification tasks.
* Retail behavior patterns are often non-linear, requiring robust models.
* Thorough model comparison is essential before deployment.

---

## 🛠 Technologies Used
* **Language:** Python
* **Libraries:** NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn
* **Environment:** Jupyter Notebook

---

## 📁 Repository Structure

```bash
├── AI_IN_RETAIL_PROJECT.ipynb    # Main source code (Jupyter Notebook)
├── README.md                     # Project documentation
├── dataset/
│   └── online_shoppers_intention.csv
└── results/
    ├── confusion_matrix.png
    ├── classification_report.txt
    └── model_comparison.png
## 📂 Project Structure

```bash
├── AI_IN_RETAIL_GRP_PROJECT.ipynb  # Main Analysis & Modeling Notebook
├── README.md                        # Project Documentation
└── online_shoppers_intention.csv    # Dataset (Source: Kaggle)

```

## ⚙️ How to Run

1. Clone the repository:
```bash
git clone https://github.com/priiyanshuraj/retailai.git

```


2. Install dependencies:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn imbalanced-learn

```


3. Open the Jupyter Notebook:
```bash
jupyter notebook AI_IN_RETAIL_GRP_PROJECT.ipynb

```



---

**Author:** Priyanshu Raj

---

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
