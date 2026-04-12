Bank Customer Churn Prediction Analysis
Author: Bilal Islamovic

Course: CIND820 - Big Data Analytics Project

Supervisor: Tamer Abdou

Dataset
Source: Kaggle Bank Customer Churn Dataset

Dataset Details:

10,000 customer records
18 features (demographics, account details, engagement metrics)
Target variable: Customer churn (20.4% baseline churn rate)
Project Overview
This analysis investigates customer churn patterns in the banking sector using machine learning techniques to identify at-risk customers and quantify financial exposure. The project addresses methodological rigor through proper validation design, feature stability analysis, and cost-benefit modeling with realistic constraints.

Research Questions
RQ1: What customer characteristics have predictive value for identifying churn risk?

RQ2: What is the financial exposure represented by customers identified as high-churn risk?

RQ3: Given assumed intervention costs and success rates, what decision threshold maximizes expected net benefit of targeted retention efforts?

Key Findings
Predictive Features: Age, number of products, account activity, and geography (Germany shows 2x churn rate)
Model Performance: Random Forest with F1-Score of 0.62 after hyperparameter tuning
Financial Exposure: $185.7M in deposits at risk from predicted churners
Optimal Strategy: Budget-constrained targeting ranked by expected loss achieves 155:1 ROI
Repository Contents

bank-churn-analysis/
├── Initial_code_and_results (7).ipynb  # Main analysis notebook
├── Customer-Churn-Records.csv          # Dataset (10,000 customers)
├── requirements.txt                     # Python dependencies
└── README.md                            # This file
How to Run This Analysis
Prerequisites
Python 3.8 or higher
Jupyter Notebook or JupyterLab
Setup Instructions
Clone the repository:


git clone https://github.com/bilalislamovic/bank-churn-analysis.git
cd bank-churn-analysis
Install dependencies:


pip install -r requirements.txt
Run the notebook:

Open Jupyter: jupyter notebook
Navigate to Initial_code_and_results (7).ipynb
Run all cells: Kernel → Restart & Run All
Expected Runtime
The complete notebook takes approximately 5-10 minutes to run on a standard laptop.

Expected Outputs
The notebook will generate:

11 visualizations (saved as PNG files)
Model performance metrics and confusion matrices
Feature importance analysis across multiple models
Financial exposure calculations
Cost-benefit analysis with budget constraints
Reproducibility
This notebook has been tested to run successfully from top to bottom without errors. All random seeds are set (random_state=42) to ensure reproducible results across runs.

Methodology
The analysis follows a structured machine learning workflow:

Exploratory data analysis with statistical validation
Feature engineering and encoding
Model comparison (Logistic Regression, Decision Tree, Random Forest)
Hyperparameter tuning with cross-validation
Model calibration for reliable probability estimates
Feature importance stability analysis
Financial impact modeling with operational constraints
All methodological choices are justified in the notebook with explicit discussion of limitations and assumptions.
