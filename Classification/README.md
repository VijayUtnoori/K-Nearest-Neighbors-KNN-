#  KNN – Breast Cancer Classification

##  Problem Statement
Build a K-Nearest Neighbors (KNN) model to classify tumors as:
- **0 → Malignant**
- **1 → Benign**

The objective is to find the optimal **K value** that gives the best classification performance.

---

##  Approach
- Loaded Breast Cancer dataset
- Split into training and testing sets
- Applied feature scaling (KNN is distance-based)
- Trained multiple models with different **K values**
- Evaluated using Accuracy, Confusion Matrix, Precision, Recall, F1-score
- Compared results to select the best K

---

##  Tested K Values
`1, 3, 5, 10, 20, 100, 200, 455`

---

##  Results

| K | Accuracy |
|---|----------|
| 1 | 0.9298 |
| 3 | 0.9386 |
| 5 | **0.9561 (Best)** |
| 10 | 0.9474 |
| 20 | 0.9386 |
| 100 | 0.9035 |
| 200 | 0.8684 |
| 455 | 0.6316 |

---

##  Best Model
**K = 5**  
Accuracy: **95.61%**

Confusion Matrix:

# [[71 1]
#[ 4 38]]
---

##  Conclusion
- Best K value: **5**
- Achieved **95.61% accuracy**
- Small K values may lead to **overfitting** (model becomes sensitive to noise).
- Very large K values may cause **underfitting** (model becomes too generalized).
- Proper K selection is critical for optimal KNN performance.



