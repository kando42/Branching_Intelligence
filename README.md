# Ground-Up Implementations of Decision Tree Algorithms

## Introduction
In this project, I implement several decision tree algorithms from scratch, including:
- **Decision Tree**
- **Bagging Classifier**
- **Random Forest**
- **AdaBoost**

The goal is to understand the inner workings of these algorithms and compare my implementations against popular libraries such as scikit-learn.

## Overview of Algorithms

### Decision Tree
- **Basic Idea:** Recursive partitioning of the dataset based on feature values.
- **Key Metrics:** Information gain, Gini impurity.

### Bagging Classifier
- **Bootstrap Aggregating:** Trains multiple independent models (often decision trees) on different bootstrap samples of the data.
- **Averaging Predictions:** Combines predictions (by voting or averaging) to reduce variance and improve model robustness.
  
### Random Forest
- **Ensemble of Decision Trees:** Aggregates the predictions of multiple trees to improve overall accuracy.
- **Feature Randomness:** Typically uses node-level feature selection to increase tree diversity.
- **Bagging:** Each tree is trained on a random bootstrap sample of the training data.
- **Comparison with Bagging Classifier:** While both methods use bagging, random forests additionally inject randomness in the feature selection at each node.
- - **Modes of Feature Selection:**
  - **Tree-Level Feature Selection:** The same subset of features is used for splitting decisions throughout the entire tree. This mode may simplify the model but can be less adaptive.
  - **Node-Level Feature Selection:** A new random subset of features is chosen at each node for splitting. This increases diversity in the splits and can reduce overfitting.

### AdaBoost
- **Boosting Algorithm:** Combines multiple weak learners (usually shallow decision trees) into a strong classifier.
- **Weighted Training Samples:** Adjusts the weights on training samples based on previous classification errors, forcing subsequent trees to focus on difficult cases.







