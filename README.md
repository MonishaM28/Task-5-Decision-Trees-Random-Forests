# Task 5: Decision Trees & Random Forests

The goal is to apply **tree-based models** (Decision Tree, Random Forest) on the **Heart Disease dataset** and demonstrate both technical and interpretability skills.

---

## 📌 Objective

* Build and evaluate **Decision Tree** and **Random Forest** models.
* Understand **overfitting** and how to control tree depth.
* Compare performance across models.
* Visualize trees, feature importances, and interpret predictions.

---

## 📊 Dataset

* **Dataset**: Heart Disease (from UCI repository).
* **Target Variable**: `target` → (1 = disease, 0 = no disease).
* **Features**: age, sex, chest pain type, blood pressure, cholesterol, max heart rate, etc.

---

## 🧪 Approach

1. **Exploratory Data Analysis (EDA)**

   * Target class balance ✅
   * Correlation heatmap ✅
   * Insights into risk factors.

2. **Modeling**

   * **Decision Tree** (visualized with Graphviz/dtreeviz).
   * **Random Forest** (ensemble model, reduces overfitting).

3. **Overfitting Analysis**

   * Depth tuning and learning curves.

4. **Evaluation**

   * Accuracy, Precision, Recall, F1, ROC-AUC.
   * Cross-validation (k=5).
   * Confusion matrices.

---

## 📈 Results (Sample – update with your runs)

| Model           | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
| --------------- | -------- | --------- | ------ | -------- | ------- |
| Decision Tree   | 78%      | 76%       | 74%    | 75%      | 0.79    |
| Random Forest   | 85%      | 84%       | 83%    | 83%      | 0.89    |

✅ Random Forest consistently outperformed a single Decision Tree.

---

## 🎨 Visuals

* **EDA Plots**
  ![Target Distribution]
  ![Correlation Heatmap]

* **Model Interpretations**
  ![Decision Tree]
  ![Feature Importances]
  ![ROC Curve]
  ![Confusion Matrix]

---

## ⚙️ Installation

```bash
pip install -r requirements.txt
```

For Colab users:

```bash
!apt-get install graphviz
```

---


## 📂 Repository Structure
```
Task5_DecisionTree_RandomForest/
│
├── data/
│   └── heart.csv
│
├── notebooks/
│   └── Task5.ipynb
│
├── requirements.txt
└── README.md
```

---

## 🏆 Conclusion

* Decision Trees are simple but prone to overfitting.
* Random Forests improve generalization significantly.



