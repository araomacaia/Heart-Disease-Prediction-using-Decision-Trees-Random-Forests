# ❤️ Heart Disease Prediction with Decision Trees & Random Forests
---
<img width="940" height="459" alt="image" src="https://github.com/user-attachments/assets/13378b75-9b5d-4fb7-a128-4527ead7c385" />

---
## 📖 Project Overview

In this project, I worked on predicting heart disease using Decision Trees and Random Forests. The dataset I used was heart.csv, which contains medical attributes like age, cholesterol level, blood pressure, and whether or not a patient is likely to have heart disease.

The objective of this task was to:

1. Train a Decision Tree Classifier and visualize the tree.

2. Understand overfitting and apply pruning by controlling max_depth.

3. Train a Random Forest Classifier and compare its performance to a single tree.

4. Interpret feature importances.

5. Evaluate the models using cross-validation and a confusion matrix.

---
## 📊 Exploratory Data Analysis

Before training, I explored the dataset and examined feature correlations.

The heatmap shows how certain variables, such as ca (number of vessels) and cp (chest pain type), are strongly correlated with the target variable.

**🌳 Decision Tree Model**

I first trained a baseline Decision Tree Classifier. The accuracy was good but the model tended to overfit.

Here’s a visualization of the trained tree (truncated at depth=3 for readability):
<img width="3547" height="1907" alt="decision_tree" src="https://github.com/user-attachments/assets/c73c977f-189e-4346-8a44-8023b9481c43" />


**✂️ Pruned Decision Tree**

To address overfitting, I limited the maximum depth of the tree (max_depth=4). This reduced variance and slightly improved generalization, though accuracy dropped a little.

**🌲 Random Forest Model**

Next, I trained a Random Forest Classifier with 100 trees. This ensemble method improved accuracy compared to the single tree and provided a more stable model.

Here’s the feature importance plot:
<img width="2641" height="1634" alt="feature_importances" src="https://github.com/user-attachments/assets/28c406db-7ef9-4fa6-b8bf-a33eab88a302" />

It shows that features like cp, thal, and ca contribute the most to predictions.

---
## 📈 Evaluation

Finally, I evaluated both models. Random Forest performed better overall.

  | Model | Accuracy (%) |
  | :------- | :------: |
  | Decision Tree    | 78 |
  | Random Forest  | 85 | 
  | Cross-validation Mean  | 83 |

The confusion matrix below shows the Random Forest’s classification results:

<img width="1558" height="685" alt="confusion_matrix_rf" src="https://github.com/user-attachments/assets/674adf7e-84d8-430e-b773-feff1db99675" />

---
## ⚙️ Tech Stack

  - Programming Language: Python

  - Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn

  - Models: Decision Tree Classifier, Random Forest Classifier

  - Environment: Jupyter Notebook

---

## 📚 Acknowledgements & References

This project was guided by several resources that helped me understand both the theory and the practical implementation of decision trees and random forests.

References Consulted:

  - Scikit-learn Developers (BSD License) Document — Decision Trees

  - Analysis of a Random Forests Model — Gérard Biau, Journal of Machine Learning Research, 2012.

  - All about Decision Trees — Abhishek Jain.

  - Decision Tree in Machine Learning — Anshuman Singh, October 16, 2024.

  - Lecture 7: Decision Trees — Alice Gao.

  - CS 446 Machine Learning, Fall 2016: Decision Trees — Prof. Dan Roth.

  - Random Forests — Leo Breiman, Statistics Dept., UC Berkeley.

  - Random Forest from Scratch: Interpreting the Math behind the Black Box.

  - Random Forest Classifiers: A Survey and Future Research Directions — Vrushali Y Kulkarni, Dr. Pradeep K Sinha.

  - Random Forest Algorithm Overview — Hasan Ahmed Salman, Ali Kalakech, Amani Steiti.

  - Random Forest Algorithm — Rohini College of Engineering and Technology.

  - Theory of Random Forests: A Review — Erwan Scornet, Giles Hooker.

---
## 📝 Author
**Arao Macaia**

AI & ML Internship Task 5 (2025)
