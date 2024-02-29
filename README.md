# Multi-class-Multi-label-classification-using-SVM

# Overview
This project explores multi-class and multi-label classification using Support Vector Machines (SVMs) on the Anuran Calls (MFCCs) dataset, alongside K-Means clustering to analyze data labeling and classification accuracy:

- **Dataset Preparation**:
  - Utilizes the Anuran Calls (MFCCs) Data Set, selecting 70% of the data randomly for the training set.

- **Multi-label Classification**:
  - **Problem Definition**: Each instance is labeled across three categories: Families, Genus, and Species, introducing a multi-class, multi-label classification challenge.
  - **Binary Relevance Approach**: Implements individual SVM classifiers for each label, employing Gaussian kernels and one-vs-all strategies, optimized via 10-fold cross-validation.
  - **Evaluation Metrics**: Examines classifiers using exact match and hamming score/loss.
  - **Standardization vs. Raw Data**: Analyzes performance differences between using standardized and raw data attributes.
  - **L1-penalized SVMs**: Explores classification with L1-penalized SVMs, necessitating attribute standardization.
  - **Class Imbalance Solutions**: Applies techniques like SMOTE to address class imbalances and evaluates their impact on classifier performance.
  - **Advanced Practices**: Investigates Classifier Chain methods and evaluates classifiers using multi-label metrics such as confusion matrices, precision, recall, ROC, and AUC.

- **K-Means Clustering on Multi-Class and Multi-Label Data**:
  - **Monte-Carlo Simulation**: Conducts 50 iterations to evaluate clustering performance, focusing on the selection of the optimal number of clusters (k) through various statistical methods.
  - **Majority Label Identification**: Identifies dominant labels within clusters for family, genus, and species.
  - **Hamming Distance Metrics**: Calculates average Hamming distance, score, and loss between true labels and cluster-assigned labels, providing a quantitative measure of clustering accuracy.

This comprehensive analysis aims to understand the intricacies of handling multi-label datasets in SVM classification and K-Means clustering, highlighting the challenges of class imbalance, the importance of optimal parameter selection, and the effectiveness of various evaluation metrics in multi-label settings.