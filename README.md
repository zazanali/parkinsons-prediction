
# 🧠 Parkinson's Disease Detection using Machine Learning

This repository presents a machine learning project focused on detecting Parkinson's Disease using voice measurement data. Parkinson’s is a progressive nervous system disorder that affects movement and can cause tremors, stiffness, and difficulty with balance and coordination.

## 📊 Problem Statement

The goal of this project is to classify whether a person is affected by Parkinson’s Disease based on various biomedical voice measurements. Early and accurate detection can help patients get timely treatment and improve quality of life.

## 📁 Dataset Information

- **Source**: [Kaggle - Parkinson Disease Detection](https://www.kaggle.com/datasets/jainaru/parkinson-disease-detection)
- **Instances**: 195
- **Features**: 22 voice-related features + 1 target column (`status`)
- **Target Column**: `status` (1 = Parkinson’s Disease, 0 = Healthy)

Each row in the dataset represents voice measurements from an individual, with features extracted from sustained phonations.

## 🔬 Features Overview

Some of the important features include:
- `MDVP:Fo(Hz)`: Average vocal fundamental frequency
- `MDVP:Jitter(%)`: Variation in fundamental frequency
- `MDVP:Shimmer`: Amplitude variation
- `NHR`, `HNR`: Noise-to-Harmonics and Harmonics-to-Noise ratios
- `spread1`, `spread2`, `DFA`, `PPE`: Nonlinear signal features

## ⚙️ Technologies Used

- Python
- Scikit-learn
- XGBoost
- Pandas, NumPy
- Matplotlib, Seaborn

## 🚀 Steps Performed

1. Data Cleaning & Preprocessing
2. Exploratory Data Analysis (EDA)
3. Feature Scaling using StandardScaler
4. Train-Test Split (80-20)
5. Model Training using XGBoost Classifier
6. Model Evaluation with classification metrics and confusion matrix

## 📈 Evaluation Metrics

Models were evaluated using:
- Accuracy Score
- Precision, Recall, F1-Score
- Confusion Matrix
- ROC-AUC Curve

## ✅ Model Results (XGBoost)

| Metric            | Value  |
|-------------------|--------|
| Accuracy          | 0.94   |
| Precision         | 0.94   |
| Recall            | 1.00   |
| F1 Score          | 0.97   |
| ROC-AUC Score     | ~0.98  |

## 📊 Confusion Matrix

|                    | Predicted Healthy | Predicted Parkinson's |
|--------------------|-------------------|------------------------|
| **Actual Healthy** | 5                 | 2                      |
| **Actual Parkinson's** | 0            | 32                     |

## 📌 How ML Helps in Parkinson’s Detection

Parkinson’s disease affects motor functions, and its symptoms reflect in a person’s speech patterns. Machine learning helps detect subtle patterns in vocal biomarkers, aiding in **early diagnosis**, even before clinical symptoms are clearly visible.

## 📉 Visualizations

- Correlation Heatmap
- Feature Importance Charts (Horizontal Bar Plot)
- Model Comparison Plots
- Confusion Matrices for each classifier

## 🔍 Conclusion

The XGBoost model achieved **94% accuracy** and **100% recall**, indicating it successfully identified all patients with Parkinson’s. Only 2 false positives were observed.

This model could assist medical professionals in pre-screening patients for Parkinson’s Disease using voice data, making diagnosis faster and more accessible.

## 📁 File Structure

- `parkinsons.ipynb` – Jupyter notebook containing the full implementation
- `README.md` – Project documentation

---

👨‍💻 Developed by: *Zazan Ali*
