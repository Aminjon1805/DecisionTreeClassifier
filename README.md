# Titanic Survival Prediction with Tree-Based Machine Learning

A machine learning project focused on understanding and comparing three popular tree-based classification algorithms on the Titanic dataset.

---

## Project Objective

The goal of this project is not only to build accurate classifiers but also to understand how different tree-based algorithms learn from data, how their hyperparameters influence performance, and how they compare under the same preprocessing pipeline.

The project includes:

- Decision Tree Classifier
- Random Forest Classifier
- XGBoost Classifier

---

## Dataset

**Dataset:** Titanic (`train.csv`)

**Problem Type:** Binary Classification

**Target Variable:** `Survived`

---

## Project Workflow

1. Load the dataset.
2. Explore the data.
3. Handle missing values.
4. Encode categorical variables.
5. Split the dataset into:
   - Training Set
   - Cross-Validation Set
   - Test Set
6. Train each model.
7. Tune hyperparameters.
8. Compare model performance.
9. Evaluate the final model on the test set.

---

# Models Implemented

## Decision Tree

- Built a baseline classifier.
- Manually tuned model complexity.
- Visualized generated trees.
- Studied overfitting and pruning.

---

## Random Forest

- Compared against a single Decision Tree.
- Tuned important hyperparameters.
- Investigated how ensembles improve generalization.
- Analyzed the effect of multiple trees on performance.

---

## XGBoost

- Implemented gradient boosting for classification.
- Used `RandomizedSearchCV` for automated hyperparameter tuning.
- Explored the impact of:
  - max_depth
  - learning_rate
  - n_estimators
  - subsample
  - colsample_bytree
  - min_child_weight
  - reg_lambda

---

# Hyperparameter Tuning

Different tuning strategies were applied throughout the project.

- Manual hyperparameter tuning
- Cross-validation model selection
- RandomizedSearchCV for XGBoost

The objective was to understand how each parameter influences model complexity, overfitting, and generalization rather than simply maximizing accuracy.

---

# Feature Engineering

**No feature engineering was performed in this project.**

The purpose of this repository is to compare the algorithms under the same preprocessing pipeline.

This makes the comparison between Decision Tree, Random Forest, and XGBoost more objective, since all models receive identical input features.

Feature engineering will be explored in future projects.

---

# Skills Practiced

- Data preprocessing
- Missing value handling
- Categorical encoding
- Model training
- Hyperparameter tuning
- Cross-validation
- Model comparison
- Performance evaluation
- Tree visualization
- Gradient Boosting
- Ensemble Learning

---

# Repository Structure

```
.
├── images/
├── DecisionTree.ipynb
├── RandomForest.ipynb
├── XGBoost.ipynb
├── train.csv
└── README.md
```

---

# Technologies

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- XGBoost

---

# Future Improvements

- Feature engineering
- Feature importance analysis
- SHAP value interpretation
- Stratified K-Fold Cross Validation
- Advanced XGBoost tuning
- Comparison after feature engineering

---

# Key Takeaways

Through this project I learned:

- How Decision Trees construct decision boundaries.
- Why Random Forest reduces overfitting through bagging.
- How XGBoost sequentially corrects previous prediction errors using gradient boosting.
- The importance of cross-validation when selecting models.
- How hyperparameter tuning affects model performance.
- When further improvement depends more on feature engineering than on additional parameter tuning.

---

## Author

**Aminjon Asoev**

This repository is part of my machine learning learning journey and documents my practical implementation of tree-based algorithms before moving on to unsupervised learning methods such as K-Means, PCA, and Anomaly Detection.
