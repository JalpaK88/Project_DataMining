# Project_DataMining

## Repository Structure

```
## Repository Structure

Project_DataMining/
├── Project_1_DM.zip   # Project 1 source files (notebook, code, etc.)
├── Project_1.pdf       # Curse of Dimensionality, Iris Dataset, PCA
├── Project_2_DM.zip   # Project 2 source files
├── Project_2.pdf       # Decision Trees, Model Overfitting, Text Classification
├── Project_3_DM.zip   # Project 3 source files
├── Project_3.pdf       # Classifier Comparison, Nonlinear SVM (NuSVC)
├── Project_4_DM.zip   # Project 4 source files
├── Project_4.pdf       # Hierarchical Clustering, K-Means, DBSCAN
└── README.md
```


# Project_DataMining

All 4 Projects covering the full data mining pipeline — from foundational concepts like dimensionality and PCA, through classification and model evaluation, to clustering and unsupervised learning on structured and unstructured data.

Each project is a Jupyter notebook (exported as PDF) containing code, visualizations, and written analysis.

## Contents

### Project 1 — Dimensionality, the Iris Dataset & PCA
- **Curse of Dimensionality:** Simulated 1,000 uniformly distributed points across 2–50 dimensions to show how the ratio of max-to-min pairwise distance collapses as dimensionality grows.
- **Iris Dataset Exploration:** Built a 4×4 scatter plot matrix of all feature pairs; designed threshold-based decision boundaries to separate the three Iris species using petal length/width, evaluating classification accuracy per species.
- **PCA:** Reduced the Iris dataset from 4 features to 2 principal components and compared class separability before and after dimensionality reduction.

### Project 2 — Decision Trees & Model Overfitting
- **Decision Tree Classifier:** Trained and cross-validated (5-fold stratified) a decision tree on the Iris dataset, achieving ~97% test accuracy; visualized the confusion matrix and the tree structure itself.
- **Overfitting/Underfitting Simulation:** Generated synthetic Gaussian + uniform data to study how training vs. testing error changes as decision tree complexity (number of leaf nodes) increases, illustrating the bias–variance tradeoff.
- **Text Classification:** Applied TF-IDF vectorization and a decision tree to classify documents from four categories of the 20 Newsgroups dataset, with confusion matrix analysis of misclassifications.

### Project 3 — Classifier Comparison & Nonlinear SVMs
- **Text Classification Benchmark:** Compared five classifiers (Linear SVC, Multinomial Naive Bayes, KNN, Random Forest, AdaBoost) on the 20 Newsgroups text classification task using TF-IDF features — Linear SVC performed best (~95% accuracy).
- **Handwritten Digit Recognition:** Built an MLP neural network classifier (96.77% accuracy) and compared it against an SVM classifier (98.78% accuracy) on the sklearn digits dataset, including confusion matrix comparison.
- **Nonlinear SVM (NuSVC):** Generated an XOR-patterned, non-linearly separable 2D dataset and classified it using a polynomial-kernel NuSVC (~96.7% accuracy), visualizing the resulting decision boundary.

### Project 4 — Clustering
- **Hierarchical Clustering:** Generated three synthetic 2D clusters and compared dendrograms across four linkage methods (ward, complete, average, single) using `AgglomerativeClustering`.
- **Clustering Handwritten Digits:** Tuned and compared K-Means and DBSCAN on the digits dataset (post PCA dimensionality reduction), evaluating performance via Adjusted Rand Index — K-Means outperformed DBSCAN on this dataset.
- **Clustering Structured (Non-linear) Data:** Applied Agglomerative Clustering (with a k-nearest-neighbors connectivity graph) and DBSCAN to a 3D Swiss Roll dataset, comparing how each algorithm handles non-linear manifold structure — DBSCAN better preserved the roll's spiral geometry.

## Tools & Libraries
Python, NumPy, pandas, Matplotlib, Seaborn, scikit-learn (classification, clustering, PCA, model selection, metrics), SciPy (hierarchical clustering)
