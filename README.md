# Federated Fraud Detection using ANN and LightGBM

## Project Overview

This project implements a ""Federated Learning-based Fraud Detection System"" using an ""Artificial Neural Network (ANN)"" and ""LightGBM"" to identify fraudulent credit card transactions. Instead of centralizing data for training, the dataset is divided into multiple simulated clients to demonstrate a federated learning environment. Local models are trained independently on each client, and their parameters are aggregated to create a global model.

The project evaluates both ANN and LightGBM using standard classification metrics such as Accuracy, Precision, Recall, F1-Score, ROC-AUC, and Confusion Matrix to compare their effectiveness in detecting fraudulent transactions.

---

## Features

* Federated Learning simulation with multiple clients
* Fraud detection using Artificial Neural Network (ANN)
* Fraud detection using LightGBM
* Data preprocessing and feature standardization
* Class imbalance handling using class weights
* Federated model aggregation (FedAvg)
* Performance evaluation using:

  * Accuracy
  * Precision
  * Recall
  * F1-Score
  * ROC-AUC Score
  * Confusion Matrix
* Comparison of ANN and LightGBM models

---

## Technologies Used

* Python
* NumPy
* Pandas
* Scikit-learn
* TensorFlow / Keras
* LightGBM
* Google Colab
* Git & GitHub

---

## Project Structure

```text
Federated-Fraud-Detection/
│
├── README.md
├── requirements.txt
├── LICENSE
├── .gitignore
│
├── notebook/
│   └── Federated_Fraud_Detection.ipynb
│
├── src/
│   └── fraud_detection.py
│
├── dataset/
│   └── README.md
│
└── results/
    ├── ann_results.txt
    ├── lightgbm_results.txt
    └── metrics_summary.txt
```

---

## Dataset

This project uses the **Credit Card Fraud Detection Dataset**.

For detailed dataset information and download instructions, refer to:

```
dataset/README.md
```

---

## Installation

### Clone the repository

```bash
git clone https://github.com/your-username/Federated-Fraud-Detection.git
```

### Navigate to the project directory

```bash
cd Federated-Fraud-Detection
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Download the dataset

Download the Credit Card Fraud Detection dataset from Kaggle and place it in the appropriate location before running the notebook or Python script.

---

## Results

### ANN Performance

| Metric    |  Value |
| --------- | -----: |
| Accuracy  |    96% |
| ROC-AUC   | 0.9718 |
| Precision |   0.04 |
| Recall    |   0.93 |
| F1-Score  |   0.08 |

### LightGBM Performance

| Metric    |  Value |
| --------- | -----: |
| Accuracy  | 99.86% |
| ROC-AUC   | 0.9441 |
| Precision |   0.55 |
| Recall    |   0.84 |
| F1-Score  |   0.67 |

### Model Comparison

* ANN achieved higher ROC-AUC and recall, identifying most fraudulent transactions.
* LightGBM significantly reduced false positives while maintaining strong fraud detection performance.
* LightGBM provided a better balance between precision and recall, making it more suitable for practical fraud detection.

---

## Future Improvements

* Implement a real Federated Learning framework such as TensorFlow Federated or Flower.
* Add Secure Aggregation and Differential Privacy techniques.
* Perform hyperparameter tuning to improve model performance.
* Deploy the trained model as a web application using Flask or FastAPI.
* Integrate explainable AI techniques such as SHAP for model interpretability.
* Extend the project with additional fraud detection datasets for broader evaluation.

---

## Author

Rahini

Final Year B.Tech (Artificial Intelligence & Machine Learning)

Interested in Machine Learning, Deep Learning, Federated Learning, and AI-based Fraud Detection.
