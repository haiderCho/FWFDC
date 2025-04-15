# Freshwater Fish Disease Classification 🐟🧠

A deep learning project for classifying freshwater fish diseases using image data. This project uses a transfer learning approach with **ResNet50** and is trained on a curated dataset of fish images from aquaculture in South Asia.

## 📝 Project Overview

Fish diseases can cause massive losses in aquaculture. Early and accurate detection is crucial for minimizing economic impact and improving fish health. This project builds a convolutional neural network model to classify images of diseased fish using **TensorFlow** and **Keras**.

## 📁 Dataset

- Source: [Kaggle - Freshwater Fish Disease Aquaculture in South Asia](https://www.kaggle.com/datasets/)
- Structure: Images categorized by disease types.
- Used `image_dataset_from_directory` with an 80/20 train-validation split.
    

## 🧠 Model Architecture

- **Base Model:** ResNet50 (with pretrained ImageNet weights)
- **Top Layers:** GlobalAveragePooling → Dense → Dropout → Dense (Softmax)
- **Input Size:** 224x224
- **Loss Function:** Categorical Crossentropy
- **Optimizer:** Adam
    

## 📊 Evaluation Metrics

- Accuracy
- F1 Score
- Precision & Recall
- ROC AUC
- Confusion Matrix
    

## 📈 Results

The model achieved high accuracy and performed well across multiple evaluation metrics. ROC curves and confusion matrices are included for visual inspection.

## 🔧 Dependencies

- Python 3.x
- TensorFlow
- Keras
- Scikit-learn
- Matplotlib, Seaborn, PIL, NumPy, Pandas
    

## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/yourusername/fwfd_classification.git
cd fwfd_classification

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook fwfd_classification.ipynb
```
