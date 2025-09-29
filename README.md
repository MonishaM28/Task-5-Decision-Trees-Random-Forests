# 🌳 Task 5: Decision Trees & Random Forests

This project is part of the **AI & ML Internship**. The goal is to apply **tree-based models** (Decision Tree, Random Forest, and XGBoost) on the **Heart Disease dataset** and demonstrate both technical and interpretability skills.

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
   * **XGBoost** (extra benchmark for better accuracy).

3. **Overfitting Analysis**

   * Depth tuning and learning curves.

4. **Evaluation**

   * Accuracy, Precision, Recall, F1, ROC-AUC.
   * Cross-validation (k=5).
   * Confusion matrices.

5. **Explainability**

   * Feature importance (RF vs XGBoost).
   * **SHAP values** → global + local explanations.

---

## 📈 Results (Sample – update with your runs)

| Model           | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
| --------------- | -------- | --------- | ------ | -------- | ------- |
| Decision Tree   | 78%      | 76%       | 74%    | 75%      | 0.79    |
| Random Forest   | 85%      | 84%       | 83%    | 83%      | 0.89    |
| XGBoost (extra) | 87%      | 85%       | 86%    | 85%      | 0.91    |

✅ Random Forest & XGBoost consistently outperformed a single Decision Tree.

---

## 🎨 Visuals

* **EDA Plots**
  ![Target Distribution](images/eda_target_distribution.png)
  ![Correlation Heatmap](images/eda_correlation_heatmap.png)

* **Model Interpretations**
  ![Decision Tree](images/decision_tree.png)
  ![Feature Importances](images/random_forest_feature_importance.png)
  ![ROC Curve](images/roc_curve.png)
  ![SHAP Summary](images/shap_summary.png)
  ![Confusion Matrix](images/confusion_matrix_rf.png)

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
├── images/
│   ├── eda_target_distribution.png
│   ├── eda_correlation_heatmap.png
│   ├── decision_tree.png
│   ├── random_forest_feature_importance.png
│   ├── roc_curve.png
│   ├── shap_summary.png
│   └── confusion_matrix_rf.png
│
├── requirements.txt
└── README.md
```

---

## 🏆 Conclusion

* Decision Trees are simple but prone to overfitting.
* Random Forests improve generalization significantly.
* XGBoost gives an extra boost in performance.
* SHAP adds **interpretability**, making the model **explainable**.

This project showcases **modeling + explainability**.
