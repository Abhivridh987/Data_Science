# Diabetes Prediction

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)](https://scikit-learn.org/)
[![XGBoost](https://img.shields.io/badge/XGBoost-AA0000?style=for-the-badge)](https://xgboost.ai/)
[![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge)](https://seaborn.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3776AB?style=for-the-badge)](https://matplotlib.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-FA0F00?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)

This project implements a machine learning model to predict diabetes based on patient health metrics. It classifies patients as diabetic or non-diabetic using features like glucose level, BMI, age, family history, etc.

## Features

- Downloads the "Diabetes Dataset" from Kaggle
- Performs feature selection using Fisher score
- Handles class imbalance by undersampling
- Encodes categorical variables
- Trains multiple classifiers: SVM, Logistic Regression, Random Forest, XGBoost
- Evaluates model performance with various metrics

## Requirements

- Python 3.x
- Required libraries:
  - numpy
  - pandas
  - seaborn
  - matplotlib
  - scikit-learn
  - xgboost
  - kagglehub

## Installation

1. Install the required Python packages:
   ```
   pip install numpy pandas seaborn matplotlib scikit-learn xgboost kagglehub
   ```

## Usage

1. Run the Python script:
   ```
   python diabetes_prediction.py
   ```

2. The script will:
   - Download the dataset from Kaggle
   - Preprocess and balance the data
   - Train multiple models
   - Print evaluation metrics

## Dataset

The project uses the "Diabetes Dataset" from Kaggle (prince7489/diabetes-dataset). It contains patient health metrics including glucose level, BMI, age, gender, family history, etc. The target variable is diabetes outcome: diabetic (1) or non-diabetic (0).

## Model

- **Preprocessing**: Categorical encoding, feature selection with Fisher score, class balancing
- **Classifiers**: 
  - Support Vector Machine (SVM) with different kernels
  - Logistic Regression
  - Random Forest Classifier
  - XGBoost Classifier
- **Evaluation**: Accuracy, confusion matrix, classification report

## Results

The script outputs accuracies and other metrics for each model. Example output:
```
SVM (linear):
Training Accuracy: 0.78
Testing Accuracy: 0.76
```

## Future Improvements

- Implement advanced feature engineering
- Add cross-validation for robust evaluation
- Experiment with neural networks
- Include hyperparameter optimization
- Add model interpretation techniques
- Deploy as a healthcare prediction tool

## License

This project is for educational purposes. Please check the dataset license on Kaggle.</content>
<parameter name="filePath">c:\Users\Abhivridh\Data_Science\ML\Projects\Diabetes\README.md