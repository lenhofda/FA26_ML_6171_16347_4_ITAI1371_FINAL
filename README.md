## FA26_ML_6171_16347_4_ITAI1371_FINAL
## Telecom Customer Churn Prediction
## ITAI 1371 – Final Machine Learning Project
## Fall 2026 | Group 4

## Project Overview
This project extends our midterm Telecom Customer Churn analysis. Our objective is to predict whether a customer will discontinue telecom services using six machine learning classification models and two ensemble approaches.

## Dataset Preparation
Prepared by Diane – Group Coordinator

The original dataset contains 7,043 customer records.

The data was split using stratified sampling:

## Dataset - Split - Records 

Training - 70% - 4,930 original; 7,244 after oversampling (Oversampling is a machine learning technique used to balance a dataset when one category has significantly fewer records than another.) 
Validation - 15% - 1,056 
Testing - 15% - 1,057 

## Midterm Corrections and Final Project Continuation

The team updated the original midterm notebook to address the professor's feedback regarding duplicate records was to retain the nine duplicate records because there were no customer IDs to establish whether they represented the same customers.  Also to switch the order of scaling and class balancing.

The final project continues from this corrected midterm notebook. All new preprocessing, classification models, ensemble methods, evaluation results, and visualizations must be incorporated into the existing notebook.

Each student responsible for classification models will train, validate, test, and document their assigned models, including performance metrics and graphs.

All team members are responsible for documenting their individual contributions and submitting their reflection journals in PDF format.

To prevent data leakage, preprocessing transformations are fitted on training data only. Oversampling is applied only to the training dataset, and the test dataset is reserved for final evaluation.

## Preprocessing includes:
One-hot encoding of categorical features. (machine learning technique that converts categorical data (words or labels) into numerical values of 0 and 1 so machine learning models can understand and process them.)

StandardScaler applied to numerical features. (machine learning preprocessing technique that standardizes numerical data so features measured on different scales can be compared fairly.)

Random oversampling applied only to training data.(machine learning technique used to balance an imbalanced dataset by randomly selecting and duplicating records from the minority class until both classes have equal numbers.)

Consistent feature columns across all three datasets.
Target variable `Churn`: 0 = No, 1 = Yes.

## Repository Files
1) `customer_churn_telecom_services.csv` – Original dataset.
2)  Updated midterm `.ipynb` notebook – Original analysis plus final-project preprocessing.
3)  `final_train.csv` – Balanced training dataset.
4)  `final_validation.csv` – Validation dataset.
5) `final_test.csv` – Held-out testing dataset.

## Team Responsibilities

 Team Member            Assignment 

Diane            Data preprocessing, GitHub coordination, project integration, and final submission 
Kei'Chara        Logistic Regression and Decision Tree 
Elquin           K-Nearest Neighbors (KNN) and Support Vector Classifier (SVC) 
Aaliyah          Random Forest and Gradient Boosting; model comparison tables, graphs, and analysis 
Seth             Voting ensemble and Bayesian ensemble; technical review with Aaliyah 

## Model Evaluation
Each classification model should report:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Required performance visualizations

Use the training dataset to fit models, the validation dataset for model selection and tuning, and the test dataset for final evaluation.

## Project Schedule

 Date            Milestone 

 November 15    Prepared datasets available to team 
 November 30    Individual models and ensemble work completed 
 December 1–4   Model review, comparison, and final integration 
 December 5     All teammates submit final work and individual reflection journals to Diane 
 December 6     Final project submitted in Canvas 

## Final Deliverables
The final GitHub repository will contain the completed notebook, original dataset, model results, ensemble comparisons, required graphs, comparison table PDF, analysis report PDF, presentation PDF (maximum four slides), and individual reflection journals in PDF format.

Collaboration note: Team members should coordinate notebook changes through separate branches and pull requests to avoid overwriting one another's work.
