# Malicious URL Detection

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)](https://scikit-learn.org/)
[![NLTK](https://img.shields.io/badge/NLTK-76B900?style=for-the-badge)](https://www.nltk.org/)
[![XGBoost](https://img.shields.io/badge/XGBoost-AA0000?style=for-the-badge)](https://xgboost.ai/)
[![Jupyter](https://img.shields.io/badge/Jupyter-FA0F00?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)

This project implements a machine learning model to detect malicious URLs using natural language processing techniques. It classifies URLs as benign or malicious (including defacement, phishing, and malware).

## Features

- Downloads the "Malicious URLs Dataset" from Kaggle
- Preprocesses URLs using TF-IDF vectorization
- Handles class imbalance by undersampling the majority class
- Trains a Logistic Regression model for binary classification
- Evaluates model performance on training and testing sets

## Requirements

- Python 3.x
- Required libraries:
  - numpy
  - pandas
  - matplotlib
  - seaborn
  - scikit-learn
  - xgboost
  - nltk
  - kagglehub

## Installation

1. Install the required Python packages:
   ```
   pip install numpy pandas matplotlib seaborn scikit-learn xgboost nltk kagglehub
   ```

2. Download NLTK stopwords (required for text processing):
   ```python
   import nltk
   nltk.download('stopwords')
   ```

## Usage

1. Run the Python script:
   ```
   python malicious_url.py
   ```

2. The script will:
   - Download the dataset from Kaggle
   - Preprocess the data
   - Train the model
   - Print training and testing accuracies

## Dataset

The project uses the "Malicious URLs Dataset" from Kaggle (sid321axn/malicious-urls-dataset). The dataset contains URLs labeled as benign, defacement, phishing, or malware. For binary classification, defacement, phishing, and malware are grouped as malicious (1), while benign is labeled as 0.

## Model

- **Vectorizer**: TF-IDF (Term Frequency-Inverse Document Frequency) to convert URLs into numerical features
- **Classifier**: Logistic Regression
- **Evaluation**: Accuracy score on training and testing sets

## Results

The script outputs the training and testing accuracies. Example output:
```
Training Accuracy: 0.95
Testing Accuracy: 0.94
```

## Future Improvements

- Experiment with other classifiers (Random Forest, XGBoost)
- Implement feature engineering for better URL analysis
- Add model persistence for deployment
- Include more evaluation metrics (precision, recall, F1-score)

## License

This project is for educational purposes. Please check the dataset license on Kaggle.