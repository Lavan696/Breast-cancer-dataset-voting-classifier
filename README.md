#  Breast Cancer Classification with Voting Classifier

This project applies a **Voting Classifier** on the **Breast Cancer dataset** from scikit-learn.  
It is a **binary classification** problem with target classes: **Malignant** and **Benign**.  
The model combines multiple classifiers to improve generalization and performance.

##  Key Features
- ✅ Split the dataset into training (80%) and testing (20%) using `train_test_split`.  
- ✅ Used a **Voting Classifier** combining:  
    - Logistic Regression  
    - Random Forest Classifier  
    - Support Vector Classifier (SVC)  
- ✅ Plotted **Confusion Matrix** and **Precision-Recall Curve** for evaluation.  
- ✅ Achieved **high recall and precision**, making the model reliable for medical diagnosis.  
- ✅ Clean, modular code structure for easy extension or experimentation with other classifiers.
- 
**Importance of Recall:**  
 In medical diagnosis, it is crucial to correctly identify all positive cases (malignant tumors).  
 A **recall score of 1.0** ensures that no malignant cases are missed, which is vital for patient safety.


## Results
- **Test Accuracy:** 96.49%  
- **Cross-Validation Score:** Mean = 96.04%  
- **Precision:** 0.94  
- **Recall:** 1.0  
- **F1 Score:** 0.97  
- **ROC AUC Score:** 0.95  



---

##  Tech Stack
- Python  
- scikit-learn  
- NumPy  
- Matplotlib  
 

---

## 📂 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/breast-cancer-voting-classifier.git
