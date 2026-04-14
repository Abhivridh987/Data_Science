# Housing Loan Prediction

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)](https://scikit-learn.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge)](https://seaborn.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3776AB?style=for-the-badge)](https://matplotlib.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-FA0F00?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)

This project implements a machine learning model to predict housing loan approval based on applicant information. It classifies loan applications as approved or rejected using features like income, credit history, education, etc.

## Features

- Loads the loan prediction dataset
- Handles categorical encoding for features like gender, education, property area
- Manages missing values by dropping null rows
- Performs feature scaling with StandardScaler
- Trains Support Vector Machine (SVM) classifier
- Evaluates model performance and visualizes data relationships

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

2. Ensure the dataset file `train_u6lujuX_CVtuZ9i (1).csv` is in the project directory or update the path in the script.

## Usage

1. Run the Python script:
   ```
   python housing_loan_prediction.py
   ```

2. The script will:
   - Load and preprocess the dataset
   - Train the SVM model
   - Print training and testing accuracies
   - Display data visualizations

## Dataset

The project uses a housing loan prediction dataset (train_u6lujuX_CVtuZ9i (1).csv). It contains applicant information including gender, marital status, education, income, loan amount, credit history, and property area. The target variable is loan status: approved (1) or rejected (0).

## Model

- **Preprocessing**: Categorical encoding, handling missing values, feature scaling
- **Classifier**: Support Vector Machine (SVM)
- **Evaluation**: Accuracy score on training and testing sets

## Results

The script outputs the training and testing accuracies. Example output:
```
Accuracy on training data: 0.82
Accuracy on test data: 0.78
```

## Future Improvements

- Experiment with other classifiers (Random Forest, Logistic Regression)
- Implement feature engineering and selection
- Add hyperparameter tuning
- Include more evaluation metrics (precision, recall, F1-score)
- Handle class imbalance if present
- Deploy the model for real-time predictions

## License

This project is for educational purposes. Please check the dataset license.</content>
<parameter name="filePath">c:\Users\Abhivridh\Data_Science\ML\Projects\Housing Loan Prediction\README.md