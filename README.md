# 🧠 Melanoma Cancer Detection using CNN

A deep learning project to detect **Melanoma** (skin cancer) from dermatoscopic images using a **Convolutional Neural Network (CNN)**. This project emphasizes **high recall**, which is crucial in medical diagnosis to reduce false negatives and catch as many true cancer cases as possible.

---

## 📌 Highlights

- 🔍 **Binary Classification**: Benign vs Malignant
- 🧠 **CNN-based Model** built with TensorFlow/Keras
- 📊 Evaluation Metrics: Accuracy, Precision, **Recall**, AUC
- 📈 Focused on improving **Recall** to reduce false negatives
- 🖼️ Real-time image prediction using Gradio Web Interface

---

## 📂 Dataset

- **Source**: [SIIM-ISIC Melanoma Classification on Kaggle](https://www.kaggle.com/competitions/siim-isic-melanoma-classification/data)
- ~40,000 high-resolution dermatoscopic images
- Labels: `1 = Melanoma`, `0 = Benign`
- Data is split into `train`, `validation`, and `test` sets


## 📊 Model Evaluation – Test Set (Threshold = 0.5)

| Metric       | Class 0 (Benign) | Class 1 (Melanoma) |
|--------------|------------------|---------------------|
| Precision    | 0.90             | 0.86                |
| Recall       | 0.85             | **0.90**            |
| F1-Score     | 0.87             | 0.88                |

- ✅ **Accuracy**: 87.5%
- 🧠 **Recall (Melanoma)**: **90.1%**
- 🎯 **Precision (Melanoma)**: 85.6%
- 📈 **AUC (ROC)**: 0.94

> ⚠️ **Why Recall matters**: In medical diagnosis, high recall means fewer false negatives, reducing the risk of undetected melanoma cases. This model is tuned to prioritize detecting every possible cancer case, even at the cost of some false positives.
