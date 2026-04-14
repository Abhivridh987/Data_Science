# Fake News Classification

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)](https://scikit-learn.org/)
[![NLTK](https://img.shields.io/badge/NLTK-76B900?style=for-the-badge)](https://www.nltk.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-FA0F00?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)

This project implements a machine learning model to classify news articles as fake or real using natural language processing techniques. It processes both the title and text content of news articles to determine their authenticity.

## Features

- Downloads the "Fake News Classification Dataset" from Kaggle
- Preprocesses text using stemming and stopword removal
- Vectorizes title and text separately using TF-IDF
- Combines features from title and text for comprehensive analysis
- Trains a Logistic Regression model for binary classification
- Evaluates model performance on training and testing sets

## Requirements

- Python 3.x
- Required libraries:
  - numpy
  - pandas
  - scikit-learn
  - nltk
  - kagglehub

## Installation

1. Install the required Python packages:
   ```
   pip install numpy pandas scikit-learn nltk kagglehub
   ```

2. Download NLTK stopwords (required for text processing):
   ```python
   import nltk
   nltk.download('stopwords')
   ```

## Usage

1. Run the Python script:
   ```
   python fake_new_detection.py
   ```

2. The script will:
   - Download the dataset from Kaggle
   - Preprocess the text data
   - Train the model
   - Print training and testing accuracies

## Dataset

The project uses the "Fake News Classification Dataset" from Kaggle (hassanamin/textdb3). The dataset contains news articles with titles and text content, labeled as 'FAKE' or 'REAL'. Labels are converted to binary: 0 for FAKE, 1 for REAL.

## Model

- **Preprocessing**: Porter Stemming and stopword removal
- **Vectorizer**: TF-IDF for both title (max_features=5000) and text (max_features=20000)
- **Feature Combination**: Horizontal stacking of title and text features
- **Classifier**: Logistic Regression
- **Evaluation**: Accuracy score on training and testing sets

## Results

The script outputs the training and testing accuracies. Example output:
```
Training Accuracy: 0.98
Testing Accuracy: 0.95
```

## Future Improvements

- Experiment with other classifiers (Random Forest, XGBoost, Neural Networks)
- Implement advanced NLP techniques (word embeddings, transformers)
- Add feature engineering for better text analysis
- Include model persistence for deployment
- Add more evaluation metrics (precision, recall, F1-score, confusion matrix)

## License

This project is for educational purposes. Please check the dataset license on Kaggle.