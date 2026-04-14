# Wine Quality Prediction

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)](https://scikit-learn.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge)](https://seaborn.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3776AB?style=for-the-badge)](https://matplotlib.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-FA0F00?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)

This project implements a machine learning model to predict wine quality based on physicochemical properties. It classifies wines as good (quality > 6) or not good using features like alcohol content, pH, citric acid, etc.

## Features

- Loads the Wine Quality dataset (WineQT.csv)
- Explores data correlations and distributions
- Performs feature engineering (e.g., pH categorization)
- Trains Random Forest Classifier and SVM with different kernels
- Evaluates model performance on training and testing sets

## Requirements

- Python 3.x
- Required libraries:
  - numpy
  - pandas
  - seaborn
  - matplotlib
  - scikit-learn

## Installation

1. Install the required Python packages:
   ```
   pip install numpy pandas seaborn matplotlib scikit-learn
   ```

2. Ensure the dataset file `WineQT.csv` is in the project directory or update the path in the script.

## Usage

1. Run the Python script:
   ```
   python wine_quality_prediction.py
   ```

2. The script will:
   - Load and preprocess the dataset
   - Train Random Forest and SVM models
   - Print training and testing accuracies for each model

## Dataset

The project uses the Wine Quality dataset (WineQT.csv). It contains physicochemical properties of red wine variants, with quality scores ranging from 0 to 10. For binary classification, wines with quality > 6 are labeled as good (1), others as not good (0).

## Model

- **Preprocessing**: Feature selection and temporary feature engineering
- **Classifiers**: 
  - Random Forest Classifier
  - Support Vector Machine (SVM) with kernels: linear, rbf, poly, sigmoid
- **Evaluation**: Accuracy score on training and testing sets

## Results

The script outputs the training and testing accuracies for each model. Example output:
```
Random Forest:
Training data Accuracy: 1.0
Testing data Accuracy: 0.85

SVM (linear):
Training data Accuracy: 0.78
Testing data Accuracy: 0.76
```

## Future Improvements

- Experiment with other classifiers (Logistic Regression, XGBoost)
- Implement hyperparameter tuning
- Add feature selection techniques
- Include more evaluation metrics (precision, recall, F1-score)
- Deploy the model as a web application

## License

This project is for educational purposes. Please check the dataset license.</content>
<parameter name="filePath">c:\Users\Abhivridh\Data_Science\ML\Projects\Wine Quality Prediction\README.md