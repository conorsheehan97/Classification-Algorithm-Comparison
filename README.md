# Classification-Algorithm-Comparison
## Overview
This project analyzes microscope images of cross-sections of 3D printed Titanium samples to classify and understand pore distribution across different gas flow rates. It compares the performance of eight Parameter Optimized Classification algorithms using a manually labeled set of 1000 ImageJ pore samples. The best performing model is then extrapolated to classify a larger, unlabeled dataset of 100,000 pores obtained at three different gas flow rates.

## Methodology
### Data Collection and Preparation:
- Microscope images processed using ImageJ software to analyze porosity, producing numeric data based on geometric features for each pore.
 - 1000 pores manually labeled into a training dataset, which is a subset of a larger set of 100,000 pores obtained at varying gas flow rates.

### Classification Algorithms:
 - Eight algorithms (K-Nearest Neighbour, Naive Bayes, Decision Trees Classifier, Support Vector Machine, Logistic Regression, Multi-Layer Perceptron, Gradient Boosted Classifier, XGBoost) evaluated for their ability to classify the training dataset.
 - Parameters optimized using GridSearchCV with cross-validation to maximize accuracy, recall, precision, and F1 score.

### Model Evaluation:
 - Average accuracy, recall, precision, and F1 score calculated for each class and overall.
 - Gradient Boosted Classifier identified as the best performing model based on evaluation metrics, with ROC and AUC analysis conducted for each class.

### Extrapolation to Larger Dataset:
 - Gradient Boosted Classifier applied to the 100,000 pore dataset to assess pore distribution across different gas flow rates.
 - Findings indicate an inverse relationship between the size and irregularity of pores (e.g., Lack of Fusion) and gas flow rate in 3D printing.

### Models Used
 - K-Nearest Neighbour
 - Naive Bayes
 - Decision Trees Classifier
 - Support Vector Machine
 - Logistic Regression
 - Multi-Layer Perceptron
 - Gradient Boosted Classifier
 - XGBoost

### Libraries Used
 - Pandas
 - Numpy
 - Scikit-learn
 - Matplotlib
 - Seaborn

## Conclusion
This project demonstrates the application of multiple classification algorithms to classify pores in 3D printed Titanium samples based on image analysis data. By leveraging machine learning techniques and parameter optimization, it identifies the Gradient Boosted Classifier as the most effective model for classifying pore types. The extrapolation of this model to a larger dataset provides insights into pore distribution trends across different gas flow rates, contributing to advancements in 3D printing quality control.

Contributions and feedback are welcome to enhance this project's capabilities and extend its applications in materials science and additive manufacturing.


