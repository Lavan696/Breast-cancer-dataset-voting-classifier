# Breast Cancer Prediction using Stacking Classifier  

## Overview  
This Machine Learning project focuses on **Breast Cancer Detection** using the built-in **Breast Cancer dataset from scikit-learn**.  
Multiple models including **Random Forest, Logistic Regression, and LinearSVC** were tuned and finally combined using a **Stacking Classifier** to achieve high performance and robust generalization.  

The primary goal of this project is to **accurately classify tumors as benign or malignant**, with particular emphasis on achieving **maximum recall** — ensuring that potential malignant cases are not missed.  

---

##  Steps Followed  

1. **Data Loading & Exploration**  
   - Loaded the dataset using `load_breast_cancer(as_frame=True)`  
   - Analyzed data distribution, feature information, and target balance.  
   - Visualized feature correlations using heatmaps and bar plots.  

2. **Data Preprocessing**  
   - Standardized all features using `StandardScaler`.  
   - Split data into training and testing sets.  

3. **Model Training & Hyperparameter Tuning**  
   - Tuned **RandomForestClassifier**, **LogisticRegression**, and **LinearSVC** using `GridSearchCV` with **StratifiedKFold (10 splits)**.  
   - Combined the top models into a **Stacking Classifier**, with Random Forest as the final estimator.  

4. **Feature Importance**  
   - Extracted and visualized the top 10 most important features based on the Random Forest model.  

5. **Model Evaluation**  
   - Used multiple evaluation metrics to validate performance, with special emphasis on **recall**.  
   - Performed **cross-validation** and visualized learning curves for performance consistency.  

6. **Model Saving**  
   - Saved the final trained model for deployment using joblib:  
     
---

## Model Performance  

| Metric                      | Score       |
|:--------------------------- |:-----------:|
| Cross-Validation Mean Score | **98.02 %** |
| Test Accuracy               | **99.12 %** |
| Precision                   | **98.61 %** |
| **Recall**                  | **100 %**   |
| f1-Score                    | **99.30 %** |
| ROC-AUC Score               | **99.54 %** |
| Log Loss                    | **0.05**    |
| Cohen’s Kappa Score         | **98.12 %** |
| Matthews Corrcoef           | **98.14 %** |

---

## Visualizations  

-  **Feature Correlation Heatmap** — Identifies relationships between numerical features.  
-  **Feature Importance Bar Plot** — Shows the top 10 most influential predictors.  
-  **Learning Curve** — Depicts training and cross-validation performance.  
-  **Calibration Curve** — Evaluates probability calibration of the stacking model.  
-  **Confusion Matrix** — Visualizes classification accuracy across classes.  
-  **ROC Curve** — Displays model discrimination capability.  
-  **Precision-Recall Curve** — Highlights trade-off between precision and recall.  
-  **Classification Report Heatmap** — Summarizes per-class performance metrics visually.  

---

## Key Insights  

- **Stacking multiple models** significantly improved overall performance.  
- **Data scaling** was essential for ensuring fair comparison among models.  
- **Emphasis on recall (100 %)** ensured that **no malignant cases were misclassified**, which is critical in healthcare diagnostics.  
- The model achieved **consistent cross-validation results**, indicating strong generalization capability.  

---

##  Tech Stack
- Python  
- scikit-learn  
- NumPy  
- Matplotlib
- Seaborn  
 

---

##  How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/breast-cancer-voting-classifier.git

---

## Author  

**Lavan kumar Konda**  
Student at NIT Andhra Pradesh  
Passionate about Machine Learning, Data Science, and AI  
LinkedIn: [https://linkedin.com/in/lavan-kumar-konda]
