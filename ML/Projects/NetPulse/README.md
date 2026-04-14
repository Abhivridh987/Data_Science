# NetPulse - Internet Quality Predictor

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)](https://scikit-learn.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge)](https://seaborn.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3776AB?style=for-the-badge)](https://matplotlib.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-FA0F00?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)

## Problem Statement

Users often connect to WiFi networks that appear strong but actually deliver poor internet service due to high latency, congestion, or packet loss. Most devices rely mainly on signal strength, which does not accurately reflect the real network performance.

## Solution

This project proposes an ML-based Internet Quality Predictor that analyzes parameters such as latency, download speed, upload speed, packet loss, and signal strength to evaluate overall internet performance and classify the connection quality into predefined categories.

## Features

- Analyzes multiple network parameters: latency, download speed, upload speed, packet loss, signal strength
- Classifies internet quality into 5 categories (0-4)
- Uses machine learning for accurate predictions
- Visualizes network performance metrics

## Internet Quality Classes

The model classifies internet quality into the following categories:

- **0 - Very Low**: Extremely poor connection with high latency (>500ms), very low speeds (<1 Mbps), high packet loss (>10%)
- **1 - Low**: Poor connection with moderate latency (200-500ms), low speeds (1-5 Mbps), moderate packet loss (5-10%)
- **2 - Medium**: Average connection with acceptable latency (100-200ms), moderate speeds (5-25 Mbps), low packet loss (2-5%)
- **3 - High**: Good connection with low latency (50-100ms), high speeds (25-50 Mbps), minimal packet loss (<2%)
- **4 - Very High**: Excellent connection with very low latency (<50ms), very high speeds (>50 Mbps), negligible packet loss (<1%)

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

2. Ensure the dataset file is available or implement data collection from network monitoring tools.

## Usage

1. Run the Python script:
   ```
   python netpulse.py
   ```

2. The script will:
   - Load network performance data
   - Train the ML model
   - Predict internet quality classes
   - Display performance metrics

## Dataset

The project requires a dataset containing network performance metrics. This could include:
- Latency (ms)
- Download speed (Mbps)
- Upload speed (Mbps)
- Packet loss (%)
- Signal strength (dBm)
- Quality labels (0-4)

## Model

- **Preprocessing**: Feature scaling and selection
- **Classifier**: Machine learning model (e.g., Random Forest, SVM, or Neural Network)
- **Evaluation**: Accuracy on quality classification

## Results

The script outputs model performance metrics and quality predictions. Example output:
```
Training Accuracy: 0.92
Testing Accuracy: 0.88

Predicted Quality for current network: 3 (High)
```

## Future Improvements

- Integrate with real-time network monitoring APIs
- Implement mobile app for on-the-go network quality assessment
- Add more sophisticated ML models (deep learning)
- Include user feedback for continuous model improvement
- Support for multiple network types (WiFi, cellular, Ethernet)
- Predictive analytics for network performance forecasting

