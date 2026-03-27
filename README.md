# Online-Shop
E-Commerce Conversion Analytics: Predictive Modeling of Purchase Intent
Author: Tanzil Mahbub

Student ID: 24147365

Domain: Predictive Consumer Analytics / Machine Learning

1. Project Overview
This repository contains a comprehensive data science pipeline designed to predict online shopper conversion. Using the Online Shoppers' Intention dataset, the project implements a Gradient Boosting Machine (GBM) to classify whether a user session will result in "Revenue" based on real-time behavioral metrics and administrative site data.

2. Technical Methodology
The core of this project is built on the Gradient Boosting Classifier, an ensemble learning technique that builds trees sequentially to minimize residual errors.

Key Pipeline Stages:
Feature Engineering: Conversion of categorical temporal data (Months, Visitor Types) into numerical indicators via One-Hot Encoding.

Data Stratification: Implementation of stratified training/testing splits to maintain the integrity of the minority class (purchasers).

Ensemble Optimization: Utilization of 100 boosting stages with a learning rate of 0.1 to capture non-linear interactions between "Page Values" and "Exit Rates."

3. Performance Metrics
The model is evaluated using three primary diagnostic visualizations to ensure clinical accuracy in a business context:

Feature Importance: Identifies the "PageValues" and "ProductRelated_Duration" as the most significant drivers of revenue.

Confusion Matrix: Measures the precision of the system in correctly identifying converting vs. non-converting users.

ROC-AUC Curve: Quantifies the model's discriminatory power, achieving a high area-under-the-curve (AUC) score.


Getty Images
4. Repository Structure
Bash
├── data/
│   └── online_shoppers_intention.csv  # Primary Dataset
├── notebooks/
│   └── conversion_analysis.ipynb      # Complete Python Implementation
├── images/
│   ├── feature_importance.png         # Figure 1
│   ├── confusion_matrix.png           # Figure 2
│   └── roc_curve.png                  # Figure 3
├── README.md                          # Project Documentation
└── LICENSE                            # MIT License
5. Requirements
To replicate this analysis, the following dependencies are required:

pandas

numpy

matplotlib

seaborn

scikit-learn

6. How to Run
Clone this repository.

Ensure online_shoppers_intention.csv is in the root directory.

Execute the Jupyter Notebook to generate the diagnostic plots and performance summary.

7. References
Sakar, C.O., et al. (2018). Real-time prediction of online shoppers’ purchasing intention. Neural Computing and Applications.

Friedman, J. H. (2001). Greedy function approximation: A gradient boosting machine. Annals of Statistics.

License: This project is licensed under the MIT License.
