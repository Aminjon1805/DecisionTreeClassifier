# Titanic Survival Prediction using Decision Tree

## Overview

This project demonstrates the complete machine learning workflow for a Decision Tree Classifier using the Titanic dataset. Instead of relying only on automated tools, the model was built and optimized manually to better understand how each hyperparameter affects model complexity and performance.

---

## Project Workflow

The project was completed in the following order:

1. Loaded and explored the dataset.
2. Removed irrelevant features.
3. Handled missing values without introducing data leakage.
4. Encoded categorical features.
5. Split the data into training, cross-validation, and test sets.
6. Trained a baseline Decision Tree.
7. Identified overfitting.
8. Manually tuned the following hyperparameters:
   - `max_depth`
   - `min_samples_split`
   - `min_samples_leaf`
   - `criterion`
   - `ccp_alpha`
   - `max_leaf_nodes`
9. Compared the manually tuned model with `GridSearchCV`.
10. Evaluated the final model on the test set.

---

## Results

### Manual Hyperparameter Tuning

| Dataset | Accuracy |
|---------|---------:|
| Train | 0.8296 |
| Cross Validation | 0.7921 |
| Test | 0.8045 |

### GridSearchCV

| Dataset | Accuracy |
|---------|---------:|
| Train | 0.8539 |
| Cross Validation | 0.7697 |
| Test | 0.7821 |

The manually tuned model achieved better validation and test accuracy while maintaining a simpler Decision Tree.

---

## What I Learned

Through this project I gained practical experience with:

- Data preprocessing
- Preventing data leakage
- Decision Tree Classification
- Hyperparameter tuning
- Overfitting analysis
- Cross-validation
- Model evaluation
- Comparing manual optimization with GridSearchCV

One of the main observations was that carefully selected manual hyperparameters produced better results than GridSearchCV on this dataset. This also provided a deeper understanding of how each Decision Tree hyperparameter influences model complexity and generalization.
---

## Conclusion

This project demonstrates the complete development of a Decision Tree classification model, from preprocessing to final evaluation. It also highlights the importance of understanding hyperparameter tuning rather than relying solely on automated optimization methods.
