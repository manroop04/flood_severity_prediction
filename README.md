
# Flood Severity Prediction Using Ensemble Machine Learning Models

This repository contains a Python implementation of flood severity prediction using various machine learning (ML) and deep learning (DL) models. The project combines individual models like Random Forest (RF), Support Vector Machines (SVM), K-Nearest Neighbors (KNN), Artificial Neural Networks (ANN), and Long Short-Term Memory networks (LSTM) into powerful ensemble methods.

## 📑 **Overview**
Flooding is a natural disaster causing significant damages. This project aims to predict flood severity levels using IoT sensor data and ensemble ML/DL models. The implemented techniques improve upon individual model performance through stacking and voting ensembles.

## 🛠️ **Features**
- **Data Preprocessing**:
  - Sampling 5% of the dataset for quick experimentation.
  - Cleaning NaN columns and rows, scaling features using MinMaxScaler.
  - Mapping categorical flood severity levels to numeric values.
- **Feature Selection**:
  - Selecting the top 20 features using the Chi-Square test.
- **Dimensionality Reduction**:
  - PCA for 2D visualization of feature clusters.
- **Models**:
  - **Individual Models**: SVM, KNN, ANN, RF, LSTM.
  - **Ensemble Models**:
    - RF + KNN
    - RF + LSTM
    - ANN + LSTM
    - LSTM + SVM
    - ANN + SVM
- **Evaluation**:
  - Accuracy and ROC-AUC metrics.
  - ROC curves for model comparisons.

## 📁 **Dataset**
The project uses a dataset (`train.csv`) containing flood sensor data with 11 input features. The target variable is `SeverityLevel` with three classes:
- **0**: Normal
- **1**: Abnormal
- **2**: High-Risk


## 🧑‍💻 **Usage**
1. Open the Jupyter Notebook or Python script to execute the workflow.
2. Models like SVM, RF, KNN, ANN, and LSTM will be trained, evaluated, and combined into ensembles.
3. Results, including performance metrics and ROC curves, will be displayed.

Here's the updated **Results** section for your README, now incorporating the new accuracy values:

---

## 📊 **Results**

### **Individual Model Performance**

| Model                | Accuracy  |
|----------------------|-----------|
| Random Forest        | 75.66%    |
| SVM                  | 88.05%    |
| KNN                  | 78.19%    |
| ANN                  | 88.92%    |
| LSTM                 | 88.62%    |

### **Ensemble Model Performance**

| Ensemble Model            | Accuracy  |
|---------------------------|-----------|
| RF + LSTM Ensemble        | 90.53%    |
| ANN + LSTM Ensemble       | 90.32%    |
| LSTM + SVM Ensemble       | 87.62%    |
| ANN + SVM Ensemble        | 89.68%    |
| RF + KNN Ensemble         | 78.76%    |

---

This **Results** section reflects the performance of both individual models and ensemble combinations. The **RF + LSTM Ensemble** outperforms all other models, with **ANN + LSTM Ensemble** coming close in accuracy.
### ROC Curves
- ROC curves for all individual and ensemble models are plotted, highlighting their comparative performance.

## 📜 **References**
Inspired by:
- *"IoT-Enabled Flood Severity Prediction via Ensemble Machine Learning Models"*, IEEE Access, 2020. [DOI: 10.1109/ACCESS.2020.2986090](https://doi.org/10.1109/ACCESS.2020.2986090)

## 📜 **License**
This project is licensed under the [MIT License](LICENSE).

