# Disease Prediction base on blood sample Parameters using Machine Learning

## Project Overview

This project focuses on building and evaluating multiple **Machine Learning classification models** to predict diseases based on blood sample parameters. The objective is to analyze model performance in terms of both **accuracy** and **execution time**, and identify the most effective algorithm for medical prediction tasks.

---

## Dataset Description

The dataset consists of various blood-related medical attributes used for prediction, including:

- Glucose level  
- Cholesterol  
- Hemoglobin  
- Platelets  
- White Blood Cells  
- Red Blood Cells  
- Hematocrit  
- Mean Corpuscular Volume (MCV)  
- Mean Corpuscular Hemoglobin (MCH)  
- Mean Corpuscular Hemoglobin Concentration (MCHC)  
- HbA1c  
- LDL & HDL Cholesterol  
- Liver enzymes (ALT, AST)  
- Heart Rate  
- Creatinine  
- Troponin  

---

## Machine Learning Models Implemented

The following algorithms were implemented and evaluated:

- Support Vector Classifier (SVC)  
- Decision Tree Classifier  
- Random Forest Classifier  
- Logistic Regression  
- K-Nearest Neighbors (KNN)  
- K-Means Clustering  
- Naive Bayes  
- XGBoost Classifier  

---

## 📈 Model Evaluation Results

### Accuracy Comparison

| Model                | Accuracy |
|---------------------|----------|
| KNN                 | 1.0000   |
| XGBoost             | 1.0000   |
| Logistic Regression | 0.8560   |
| Random Forest       | 0.8301   |
| SVC                 | 0.8132   |
| Decision Tree       | 0.8004   |
| Naive Bayes         | 0.4798   |
| K-Means             | 0.0000   |

---

### Execution Time Comparison

| Model                | Time (seconds) |
|---------------------|----------------|
| SVC                 | 12.96          |
| Decision Tree       | 10.83          |
| Random Forest       | 9.41           |
| Logistic Regression | 6.59           |
| KNN                 | 8.73           |
| K-Means             | 1.84           |
| Naive Bayes         | 2.44           |
| XGBoost             | 7.89           |

---

## Key Findings

- **KNN and XGBoost** achieved the highest accuracy (1.0), indicating strong predictive capability on this dataset.
- **Logistic Regression** provided a strong balance between accuracy and computational efficiency.
- **K-Means** performed poorly for classification tasks, as expected since it is an unsupervised algorithm.
- **Naive Bayes** showed comparatively lower performance due to dataset complexity.
- Trade-off between **model accuracy and execution time** is clearly observed across algorithms.

---

## Technologies Used

- Python  
- NumPy & Pandas  
- Scikit-learn  
- XGBoost  
- Matplotlib & Seaborn  
- Google Colab  

---

## Project Workflow

1. Data Preprocessing & Cleaning  
2. Exploratory Data Analysis (EDA)  
3. Feature Selection  
4. Model Training  
5. Model Evaluation  
6. Performance Comparison  

---

## Conclusion

Based on the evaluation of multiple machine learning algorithms on the blood sample dataset, model performance was compared using both accuracy and execution time as key metrics.

The results indicate that XGBoost and K-Nearest Neighbors (KNN) achieved the highest accuracy of 1.0. However, from a practical and methodological standpoint, KNN achieving perfect accuracy may suggest potential issues such as data leakage, overfitting, or dataset simplicity, and therefore requires careful validation before deployment.

Among all evaluated models, XGBoost is identified as the most reliable and robust model, as it consistently performs well on structured medical datasets, offers strong generalization capability, and maintains a good balance between accuracy and computational efficiency.

---

## Future Improvements

- Hyperparameter tuning for all models  
- Cross-validation for better reliability  
- Feature engineering and selection optimization  
- Deployment using Flask / Streamlit for real-world use  
