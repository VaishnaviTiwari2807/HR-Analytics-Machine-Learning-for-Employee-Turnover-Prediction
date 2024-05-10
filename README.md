# Human-Resources-Department-Solution


## Overview
This project is designed to address critical challenges faced by Human Resources (HR) departments in hiring and retaining employees efficiently. By leveraging data science techniques, this project aims to predict which employees are more likely to quit. This predictive model assists HR in making informed decisions, ultimately saving time and reducing costs associated with employee turnover.

## Project Structure
- **Human_Resources_Department_Solution.ipynb**: The main Jupyter Notebook containing all data analyses, model building, and evaluations.
- **data/**: This directory contains datasets used for model training and testing.
- **requirements.txt**: A text file listing the libraries required to run the project.

## Features
- **Data Exploration**: Analyze employee data to understand factors influencing employee turnover.
- **Model Building**: Implements several machine learning algorithms including:
  - Logistic Regression
  - Random Forest Classifier
  - XGBoost Classifier
- **Model Evaluation**: Uses metrics like accuracy, precision, recall, F1-score, and confusion matrices to evaluate model performance.
## Model Evaluation

The performance of each model was evaluated using precision, recall, f1-score, and overall accuracy. Below is a summary of how each model performed on the test dataset:

### Logistic Regression
- **Accuracy**: 89%
- **Precision**: 76% (for class 1)
- **Recall**: 45% (for class 1)
- **F1-Score**: 57% (for class 1)

### Decision Tree Classifier
- **Accuracy**: 80%
- **Precision**: 38% (for class 1)
- **Recall**: 38% (for class 1)
- **F1-Score**: 38% (for class 1)

### Random Forest Classifier
- Initial Model:
  - **Accuracy**: 86%
  - **Precision**: 69% (for class 1)
  - **Recall**: 16% (for class 1)
  - **F1-Score**: 25% (for class 1)
- Tuned Model (50 estimators, entropy criterion):
  - **Training Set Accuracy**: 100%
  - **Test Set Accuracy**: 86%
  - **Test Set Precision**: 75% (for class 1)
  - **Test Set Recall**: 16% (for class 1)
  - **Test Set F1-Score**: 26% (for class 1)

### XGBoost Classifier
- **Accuracy**: 86%
- **Precision**: 67% (for class 1)
- **Recall**: 28% (for class 1)
- **F1-Score**: 39% (for class 1)

### Summary
The Logistic Regression model showed the highest precision and f1-score for predicting class 1, which is critical for predicting employee attrition effectively. While the Random Forest and XGBoost models provided competitive accuracy, their recall rates for class 1 were lower, which could result in missing potential attrition cases. Decision Tree model demonstrated lower performance across all metrics compared to other models.

Given these insights, Logistic Regression stands out as a robust choice for this specific HR task, balancing accuracy with precision and recall effectively. However, for scenarios prioritizing the detection of all potential attritions, adjustments in model parameters or ensemble methods could be explored to improve recall scores.


## Getting Started

### Prerequisites
Ensure you have Python installed on your machine (preferably Python 3.8 or above). You will also need Jupyter Notebook or JupyterLab to run the `.ipynb` file.

### Installation
 **Clone the repository or download the project files:**

