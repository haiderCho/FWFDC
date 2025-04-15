<h1 align="center"> Freshwater Fish Disease Classification </h1>
<h2 align="center">
<p align="center">
 <img alt="Languages" src="https://img.shields.io/github/languages/count/haiderCho/FWFDC">
 <img alt="Repository size" src="https://img.shields.io/github/repo-size/haiderCho/FWFDC">
 <img alt="Contributors" src="https://img.shields.io/github/contributors/haiderCho/FWFDC">
 <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/haiderCho/FWFDC">
</p>
</h2>

This project uses deep learning and transfer learning with ResNet50 to classify freshwater fish diseases from images, trained on a curated dataset from aquaculture in South Asia.

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
