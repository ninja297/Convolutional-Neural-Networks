# Convolutional Neural Networks Lab

This repository contains my end-to-end CNN lab assignment work in a single Jupyter notebook:
[CNN_Lab_main.ipynb](./CNN_Lab_main.ipynb)

The project covers the full workflow from data preparation and CNN fundamentals to training, interpretability, and transfer learning. All tasks were completed with reproducibility in mind using a fixed random seed of `42`.

## Notebook Scope

The notebook currently includes:

- environment setup and package verification
- MNIST and CIFAR-10 dataset exploration
- preprocessing and augmentation pipelines
- manual 2D convolution using NumPy
- LeNet-5 implementation and parameter analysis
- a custom CIFAR-10 CNN architecture
- optimiser, learning-rate, batch-size, and regularisation experiments
- filter visualisation, feature maps, Grad-CAM, and confusion analysis
- transfer learning with a pre-trained ResNet50 backbone

## Main Files

- `CNN_Lab_main.ipynb`: master notebook containing all written answers, code, outputs, and plots
- `dataset_samples.png`: MNIST and CIFAR-10 sample grid
- `augmentation_demo.png`: CIFAR-10 augmentation examples
- `lenet_sgd_curves.png`: Task 3 first training run curves
- `optimiser_comparison.png`: optimiser comparison plot
- `regularisation_experiment.png`: regularisation comparison curves
- `lr_schedule_comparison.png`: learning-rate scheduler comparison
- `conv1_filters.png`: first-layer learned filters
- `fmaps_layer1.png`: early-layer feature maps
- `fmaps_last.png`: last-layer feature maps
- `gradcam_results.png`: Grad-CAM visualisation results
- `confusion_matrix.png`: CIFAR-10 confusion matrix
- `most_confused_examples.png`: examples from the most confused class pair
- `tl_frozen.png`: frozen-base transfer learning curve
- `tl_finetuned.png`: gradual fine-tuning curve

## Tasks Overview

### Task 1: Environment Setup & Data Pipeline

- verified the deep learning environment
- explored MNIST and CIFAR-10 shapes, dtypes, and value ranges
- implemented manual preprocessing
- built a training-only augmentation pipeline

### Task 2: Building a CNN from Scratch

- implemented manual convolution with NumPy
- derived output sizes analytically
- built LeNet-5
- designed a custom CNN for CIFAR-10

### Task 3: Training, Tuning & Regularisation

- trained LeNet-5 on MNIST
- compared SGD, SGD with momentum, and Adam
- ran a learning-rate and batch-size grid search
- compared regularisation strategies
- evaluated learning-rate scheduling

### Task 4: Visualisation & Interpretability

- visualised first-layer filters
- compared intermediate feature maps
- implemented Grad-CAM from scratch
- generated a confusion matrix and classification report

### Task 5: Transfer Learning & Fine-Tuning

- used a pre-trained ResNet50 as a frozen feature extractor
- fine-tuned the final convolutional layers with a smaller learning rate
- compared transfer learning against training from scratch

## Frameworks and Libraries

This project uses:

- Python
- TensorFlow / Keras
- PyTorch
- NumPy
- Matplotlib
- scikit-learn

The heavier transfer-learning experiments were run with GPU-enabled PyTorch for faster execution.

## Reproducibility

- random seed fixed to `42`
- outputs saved directly from notebook cells
- figures stored in the repository with the filenames required by the assignment

## How to Open

1. Clone the repository.
2. Open `CNN_Lab_main.ipynb` in Jupyter Notebook, JupyterLab, or VS Code.
3. Run cells from top to bottom if you want to reproduce the outputs locally.

## Notes

- This repository is structured around the notebook rather than separate Python modules.
- Some helper scripts may exist locally during development, but the notebook and saved figures are the primary submission artifacts.

