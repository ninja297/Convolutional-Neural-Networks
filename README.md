# 📌 Convolutional Neural Networks Lab Assignment

## 🚀 Overview
This repository contains my complete implementation of a Convolutional Neural Networks (CNN) Lab Assignment as part of a Machine Learning / Deep Learning course.

The project covers the full CNN pipeline — from data preprocessing to transfer learning — including manual implementation and model interpretability.

---

## 🧠 Key Features
- Built CNN from scratch using NumPy
- Implemented LeNet-5 architecture
- Designed a custom CNN for CIFAR-10
- Performed training, tuning & regularisation
- Visualised filters, feature maps & Grad-CAM
- Applied transfer learning (VGG16 / ResNet50)
- Compared scratch vs pretrained models

---

## 📂 Dataset
- MNIST (Handwritten digits)
- CIFAR-10 (Object classification)

---

## ⚙️ Tech Stack
- Python
- TensorFlow / Keras (or PyTorch)
- NumPy
- Matplotlib
- Scikit-learn

---

## 📁 Project Structure
cnn-lab-assignment/
│
├── Task1_Data_Pipeline/
├── Task2_CNN_From_Scratch/
├── Task3_Training_Tuning/
├── Task4_Visualization/
├── Task5_Transfer_Learning/
│
├── outputs/
│   ├── dataset_samples.png
│   ├── augmentation_demo.png
│   ├── lenet_sgd_curves.png
│   ├── optimiser_comparison.png
│   ├── gradcam_results.png
│   └── ...
│
└── README.md

---

## 🧩 Tasks Breakdown

### 🔹 Task 1: Environment & Data Pipeline
- Dataset loading and exploration
- Data preprocessing (normalisation, reshaping, encoding)
- Data augmentation

### 🔹 Task 2: CNN from Scratch
- Manual 2D convolution using NumPy
- Implemented LeNet-5
- Designed custom CNN architecture

### 🔹 Task 3: Training & Regularisation
- Optimiser comparison (SGD, Momentum, Adam)
- Learning rate and batch size tuning
- Regularisation: Dropout, BatchNorm
- Learning rate scheduling

### 🔹 Task 4: Visualisation & Interpretability
- Filter visualisation
- Feature maps extraction
- Grad-CAM implementation
- Confusion matrix & classification report

### 🔹 Task 5: Transfer Learning
- Pretrained models (VGG16 / ResNet50)
- Feature extraction vs fine-tuning
- Layer unfreezing experiments
- Performance benchmarking

---

## 📊 Results
- High accuracy achieved on MNIST and CIFAR-10
- Transfer learning improved performance significantly
- Better generalisation with regularisation techniques

---

## 🛠️ How to Run

# Clone the repository
git clone https://github.com/your-username/cnn-lab-assignment.git

# Navigate to project
cd cnn-lab-assignment

# Install dependencies
pip install -r requirements.txt

# Run Jupyter Notebook
jupyter notebook

---

## 📌 Key Learnings
- CNNs learn hierarchical features (edges → shapes → objects)
- Small kernels improve efficiency
- Regularisation prevents overfitting
- Transfer learning boosts performance on small datasets
- Grad-CAM helps interpret model predictions

---

## 📎 Submission Details
- All tasks implemented from scratch
- Reproducible results (random seed = 42)
- Includes plots, analysis, and model summaries

---

## 🤝 Acknowledgment
This project was completed as part of an academic lab assignment. All implementations are original and built independently.

---
