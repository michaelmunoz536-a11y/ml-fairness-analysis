ML Fairness Analysis

Comparative analysis of Logistic Regression, Random Forest, and XGBoost models using fairness and performance metrics across healthcare and diversity datasets.

Overview

This project evaluates the relationship between machine learning model performance and fairness across two different datasets:

A synthetic healthcare patient dataset
A diversity in tech companies dataset

The project investigates how dataset structure and demographic representation can influence both prediction accuracy and bias in machine learning systems.

Three classification models were analyzed:

Logistic Regression
Random Forest Classifier
XGBoost

The study compares model effectiveness using traditional performance metrics while also evaluating fairness outcomes across demographic groups.

Objectives
Compare machine learning model performance across multiple datasets
Evaluate fairness and bias within model predictions
Analyze how dataset characteristics affect outcomes
Apply fairness metrics to measure demographic disparities
Explore bias mitigation techniques
Technologies Used
Python
Pandas
NumPy
Scikit-learn
XGBoost
Matplotlib
Seaborn
Jupyter Notebook
Machine Learning Models
Logistic Regression

Used as a baseline linear classification model for comparison.

Random Forest Classifier

Ensemble learning model used to improve prediction stability and reduce variance.

XGBoost

Gradient boosting model used for high-performance classification analysis.

Datasets
1. Synthetic Healthcare Patient Journey Dataset

This dataset simulates patient healthcare experiences and includes features such as:

Age
Gender
Admission type
Department
Treatment intensity
Readmission status

The dataset was used to predict 30-day hospital readmission outcomes.

2. Diversity in Tech Companies Dataset

This dataset contains demographic information from technology companies, including:

Gender representation
Racial representation
Workforce diversity statistics

The dataset was used to analyze fairness and demographic prediction disparities.

Performance Metrics

The following metrics were used to evaluate model performance:

Accuracy
Precision
Recall
F1-Score
ROC-AUC
Fairness Metrics

To evaluate ethical concerns and demographic disparities, the following fairness metrics were analyzed:

Demographic Parity
Equal Opportunity
Equalized Odds
Disparate Impact
Bias Mitigation Techniques

Several preprocessing and mitigation techniques were tested to reduce model bias:

Suppression
Reweighing
Sampling
Massaging

The results demonstrated that some mitigation techniques improved fairness while slightly affecting model performance.

Key Findings
Logistic Regression achieved the strongest ROC-AUC performance on both datasets.
High model accuracy did not guarantee fairness across demographic groups.
The diversity dataset revealed stronger demographic disparities than the healthcare dataset.
Dataset structure and representation significantly influenced fairness outcomes.
Bias mitigation techniques reduced disparities but introduced trade-offs between fairness and accuracy.
Repository Structure
ml-fairness-analysis/
│
├── data/
│   ├── healthcare_patient_journey.csv
│   └── diversity_in_tech_companies.csv
│
├── notebooks/
│   ├── healthcare-analysis.ipynb
│   ├── diversity-analysis.ipynb
│   └── fairness-metrics-analysis.ipynb
│
├── images/
│   ├── roc-curve.png
│   ├── confusion-matrix.png
│   └── fairness-metrics.png
│
├── report/
│   └── fairness-performance-analysis.pdf
│
├── README.md
├── requirements.txt
└── LICENSE
Installation

Clone the repository:

git clone https://github.com/yourusername/ml-fairness-analysis.git

Install required dependencies:

pip install -r requirements.txt
Running the Project

Open the notebooks using Jupyter Notebook or VS Code:

jupyter notebook

Run the notebooks inside the notebooks/ directory to reproduce the analysis and visualizations.

Visualizations Included
ROC Curve Comparisons
Confusion Matrices
Demographic Parity Charts
Equal Opportunity Analysis
Equalized Odds Comparisons
Correlation Heatmaps
Ethical Considerations

Machine learning systems can unintentionally reproduce demographic inequalities present in training data. This project highlights the importance of evaluating fairness alongside predictive performance when developing AI systems used in healthcare, workforce analytics, and decision-making environments.

Future Improvements
Evaluate additional fairness metrics
Test more advanced bias mitigation techniques
Expand analysis using real-world datasets
Explore deep learning fairness applications
Deploy interactive dashboards for visualization
Authors
Michael Munoz
Will Fisher
License

This project is licensed under the MIT License.
