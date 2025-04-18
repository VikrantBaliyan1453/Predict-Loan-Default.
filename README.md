# Predict-Loan-Default.

 Methodology

1. Data Preprocessing
   - Dropped irrelevant columns (e.g., LoanID)
   - Encoded categorical features with `LabelEncoder`

2. Train-Test Split
   - Split data: 80% training / 20% testing

3. Modeling
   - Used `RandomForestClassifier` from `scikit-learn`
   - Trained on preprocessed data

4. Evaluation
   - Generated a confusion matrix
   - Calculated classification metrics

---

 Sample Output

Confusion Matrix

|                       | Predicted No Default | Predicted Default |
|-----------------------|----------------------|-------------------|
| **Actual No Default** | 45,000               | 170               |
| **Actual Default**    | 5,617                | 283               |

### Classification Report


The model shows high accuracy but struggles to correctly recall default cases (due to class imbalance).

---

Future Improvements

- Address **class imbalance** using:
  - SMOTE (Synthetic Minority Over-sampling Technique)
  - Class weights in the classifier
- Try other models: XGBoost, Logistic Regression
- Hyperparameter tuning

---

References

- [Scikit-learn](https://scikit-learn.org/)
- [Seaborn](https://seaborn.pydata.org/)
- [Matplotlib](https://matplotlib.org/)
- Dataset: Provided by user

---

Author

[Vikrant Baliyan] 
Machine Learning Enthusiast

---

