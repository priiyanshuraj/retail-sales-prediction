🛒 Online Shoppers Purchase Intention Prediction using Machine Learning
📌 Project Overview

This repository contains an academic machine learning project focused on predicting whether an online shopper will make a purchase (Revenue = True/False) based on their browsing behavior.

The project applies data preprocessing, exploratory data analysis (EDA), and multiple classification models, followed by a comparative performance evaluation to determine the most effective algorithm.

🎯 Project Objectives

To analyze real-world e-commerce user behavior data

To preprocess and clean a structured retail dataset

To implement multiple machine learning classification models

To compare models using standard evaluation metrics

To identify the best-performing model for purchase prediction

📊 Dataset Description

Dataset: Online Shoppers Intention Dataset

Source: Kaggle

Total Records: ~12,000 user sessions

Target Variable: Revenue

True → Purchase made

False → No purchase

Key Features:

Page visit counts (Administrative, Informational, ProductRelated)

Time spent on each page category

Bounce Rate and Exit Rate

Browser, Region, Traffic Type

Weekend indicator

🧹 Data Preprocessing

The following steps were performed:

Removal of duplicate entries

Validation of missing values

Conversion of integer-coded categorical features into categorical types

Dataset inspection using .info() and .describe()

Train–test split for unbiased evaluation

These steps ensured data quality and model reliability.

🧠 Machine Learning Models Implemented

The project focuses on classification algorithms:

Logistic Regression

Decision Tree Classifier

Random Forest Classifier

All models were trained and tested using the same dataset split to ensure a fair comparison.

📈 Evaluation Metrics Explained

The models were evaluated using the following metrics:

🔹 Accuracy

Percentage of total predictions that were correct.

🔹 Precision

Out of all predicted purchases, how many were actually purchases.

🔹 Recall

Out of all actual purchases, how many were correctly identified.

🔹 F1-Score

Harmonic mean of Precision and Recall.
Useful when class distribution is imbalanced.

🔹 Confusion Matrix

Shows correct and incorrect predictions across both classes.

📊 Model Performance Results
🔢 Classification Report Summary
Model	Accuracy	Precision	Recall	F1-Score
Logistic Regression	0.84	0.79	0.56	0.65
Decision Tree	0.86	0.73	0.68	0.70
Random Forest	0.90	0.84	0.71	0.77
📌 Interpretation of Results
Logistic Regression

Performs well as a baseline model

High interpretability

Lower recall indicates missed purchase predictions

Decision Tree

Captures non-linear patterns

Improved recall compared to Logistic Regression

Shows signs of overfitting

Random Forest (Best Model)

Highest accuracy and F1-score

Best balance between precision and recall

Reduced overfitting due to ensemble learning

🏆 Final Conclusion

✅ Random Forest Classifier is the best-performing model for this dataset.

This confirms that:

Ensemble methods outperform single estimators

Complex retail behavior patterns require non-linear models

Model comparison is essential before deployment

🛠 Technologies Used

Python

NumPy

Pandas

Matplotlib

Seaborn

Scikit-learn

Jupyter Notebook


📚 Academic Declaration

This project was developed as part of a college academic curriculum to gain hands-on experience in machine learning model development, evaluation, and comparative analysis using a real-world retail dataset.

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
