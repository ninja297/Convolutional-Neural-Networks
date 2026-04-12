📌 Convolutional Neural Networks Lab Assignment
🚀 Overview

This repository contains my complete implementation of a Convolutional Neural Networks (CNN) Lab Assignment as part of a Machine Learning / Deep Learning course.

The project covers the full CNN pipeline—from data preprocessing to transfer learning, including manual implementation and interpretability techniques.

🧠 Key Highlights
✅ Built CNN from scratch using NumPy
✅ Implemented LeNet-5 architecture
✅ Designed a custom CNN for CIFAR-10
✅ Performed training, tuning & regularisation experiments
✅ Visualised filters, feature maps & Grad-CAM
✅ Applied transfer learning (VGG16 / ResNet50)
✅ Compared scratch vs pretrained models
📂 Dataset Used
MNIST – Handwritten digit classification
CIFAR-10 – 10-class object classification
⚙️ Tech Stack
Python 🐍
TensorFlow / Keras (or PyTorch – update accordingly)
NumPy
Matplotlib
Scikit-learn
📊 Project Structure
├── Task1_Data_Pipeline/
├── Task2_CNN_From_Scratch/
├── Task3_Training_Tuning/
├── Task4_Visualization/
├── Task5_Transfer_Learning/
├── outputs/
│   ├── dataset_samples.png
│   ├── augmentation_demo.png
│   ├── lenet_sgd_curves.png
│   ├── optimiser_comparison.png
│   ├── gradcam_results.png
│   └── ...
└── README.md
🧩 Tasks Breakdown
🔹 Task 1: Environment & Data Pipeline
Dataset loading (MNIST, CIFAR-10)
Data preprocessing (normalisation, reshaping, encoding)
Data augmentation
🔹 Task 2: CNN from Scratch
Manual 2D convolution (NumPy only)
Implemented LeNet-5
Designed custom CNN architecture
🔹 Task 3: Training & Regularisation
Optimiser comparison (SGD, Momentum, Adam)
Learning rate & batch size tuning
Regularisation techniques:
Dropout
Batch Normalisation
L2 Regularisation
Learning rate scheduling
🔹 Task 4: Visualisation & Interpretability
Filter visualisation
Feature map extraction
Grad-CAM implementation (from scratch)
Confusion matrix & classification report
🔹 Task 5: Transfer Learning
Pretrained models (VGG16 / ResNet50)
Feature extraction vs fine-tuning
Layer unfreezing experiments
Benchmark comparison:
Scratch vs Transfer Learning
📈 Results
Achieved strong performance on both MNIST & CIFAR-10
Transfer learning significantly improved:
Faster convergence ⚡
Higher validation accuracy 📊
📌 Key Learnings
CNNs learn hierarchical features (edges → shapes → objects)
Small kernels (3×3) are more efficient than large ones
Regularisation is critical to avoid overfitting
Transfer learning is powerful for small datasets
Grad-CAM helps interpret model decisions
🛠️ How to Run
# Clone the repo
git clone https://github.com/your-username/cnn-lab-assignment.git

# Navigate
cd cnn-lab-assignment

# Install dependencies
pip install -r requirements.txt

# Run notebook
jupyter notebook
📎 Submission Details
All tasks implemented from scratch
Results reproducible (random seed = 42)
Includes plots, analysis, and model summaries
🤝 Acknowledgment

This project was completed as part of an academic lab assignment. All implementations are original and built without copying external code.
