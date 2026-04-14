# Convolutional Neural Networks Lab Assignment

## Student Details

- **Name:** Saloni Kushwaha
- **Roll Number:** 24it3045

## Overview

This repository contains my complete Convolutional Neural Networks lab assignment in a single Jupyter notebook:
[CNN_Lab_main.ipynb](./CNN_Lab_main.ipynb)

The work covers the full pipeline of CNN-based image classification, starting from environment setup and dataset inspection, moving through manual convolution and custom CNN design, and ending with interpretability and transfer learning. The notebook includes code, outputs, written observations, plots, and reflection answers required for submission.

The assignment uses both **MNIST** and **CIFAR-10** and combines **TensorFlow/Keras** and **PyTorch** where appropriate. Early tasks were completed with TensorFlow/Keras, while the heavier transfer-learning experiments were completed with **GPU-enabled PyTorch** for faster execution.

## Submission Contents

The main submission artifact is:

- `CNN_Lab_main.ipynb`

Supporting figures generated during the notebook include:

- `dataset_samples.png`
- `augmentation_demo.png`
- `lenet_sgd_curves.png`
- `optimiser_comparison.png`
- `regularisation_experiment.png`
- `lr_schedule_comparison.png`
- `conv1_filters.png`
- `fmaps_layer1.png`
- `fmaps_last.png`
- `gradcam_results.png`
- `confusion_matrix.png`
- `most_confused_examples.png`
- `tl_frozen.png`
- `tl_finetuned.png`
- `tl_benchmark.png`

## Datasets Used

### MNIST

Used for:

- dataset exploration
- preprocessing checks
- LeNet-5 implementation
- first training experiments
- optimiser comparison

### CIFAR-10

Used for:

- dataset exploration
- augmentation pipeline
- custom CNN design
- tuning and regularisation experiments
- interpretability experiments
- transfer learning and fine-tuning

## Task-Wise Summary

### Task 1: Environment Setup & Data Pipeline

This section establishes the working deep learning environment and prepares the datasets for later CNN tasks.

Completed work:

- verified package versions and hardware availability
- set all random seeds to `42` for reproducibility
- checked whether GPU support was available
- loaded MNIST and CIFAR-10 datasets
- inspected shapes, data types, and raw pixel ranges
- checked MNIST class balance
- built a manual preprocessing pipeline
- normalized images to `[0, 1]`
- reshaped MNIST from `(N, 28, 28)` to `(N, 28, 28, 1)`
- applied one-hot encoding to labels
- created a CIFAR-10 augmentation pipeline with flip, rotation, and zoom

Generated outputs:

- `dataset_samples.png`
- `augmentation_demo.png`

### Task 2: Building a CNN from Scratch

This section focuses on core CNN mechanics and architecture design.

Completed work:

- implemented a manual 2D convolution function using NumPy only
- computed the numerical feature map for the given Sobel-style kernel
- derived output sizes analytically using the convolution formula
- implemented LeNet-5 from the architecture description
- printed the model summary
- manually verified parameter calculations
- designed an original custom CNN for CIFAR-10
- included an ASCII architecture sketch and design rationale

Key architectural work:

- LeNet-5 for MNIST
- custom CNN for CIFAR-10 with convolution blocks, batch normalization, pooling, dropout, and classification head

### Task 3: Training, Tuning & Regularisation

This section evaluates model training behaviour under different optimisation and regularisation settings.

Completed work:

- trained LeNet-5 on MNIST for the first full run
- plotted training and validation loss
- plotted training and validation accuracy
- identified overfitting behaviour
- reported test accuracy
- compared three optimisers:
  - SGD
  - SGD with momentum
  - Adam
- performed a grid search over learning rate and batch size
- compared four regularisation settings on CIFAR-10:
  - no regularisation
  - dropout only
  - batch normalization only
  - dropout + batch normalization
- compared two learning-rate schedulers:
  - ReduceLROnPlateau
  - Cosine Annealing

Generated outputs:

- `lenet_sgd_curves.png`
- `optimiser_comparison.png`
- `regularisation_experiment.png`
- `lr_schedule_comparison.png`

Important observations from this section:

- momentum and Adam converged faster than plain SGD
- regularisation strongly affected train-validation gap
- scheduler choice changed validation behaviour over training

### Task 4: Visualisation & Interpretability

This section explores what the CIFAR-10 CNN learns internally and how its predictions can be interpreted.

Completed work:

- visualised learned filters from the first convolutional layer
- displayed early-layer and late-layer feature maps
- implemented Grad-CAM from scratch
- generated Grad-CAM visualisations for correctly classified and misclassified examples
- computed and plotted the confusion matrix
- generated the classification report
- identified strongest and weakest classes
- identified the most confused class pair
- visualised misclassified samples from that confusion pair

Generated outputs:

- `conv1_filters.png`
- `fmaps_layer1.png`
- `fmaps_last.png`
- `gradcam_results.png`
- `confusion_matrix.png`
- `most_confused_examples.png`

Representative findings:

- early filters learned edge, texture, and color-contrast style patterns
- early feature maps were visually interpretable, while deeper maps became more abstract
- Grad-CAM helped show whether the model was focusing on the object or distracting background regions

### Task 5: Transfer Learning & Fine-Tuning

This section compares training from scratch with transfer learning using a pre-trained ImageNet backbone.

Completed work:

- used a pre-trained `ResNet50` as a frozen feature extractor
- resized CIFAR-10 images to `96 x 96`
- applied the model’s recommended preprocessing
- trained only the custom head for 10 epochs
- unfroze the last 4 convolutional layers and fine-tuned with a smaller learning rate
- applied early stopping during fine-tuning
- performed an ablation study for:
  - top 2 layers unfrozen
  - top 8 layers unfrozen
  - all layers unfrozen
- benchmarked three setups:
  - scratch CNN
  - frozen pre-trained base
  - fine-tuned pre-trained base

Generated outputs:

- `tl_frozen.png`
- `tl_finetuned.png`
- `tl_benchmark.png`

Key benchmark results:

- scratch CNN test accuracy: `0.7195`
- frozen pre-trained base test accuracy: `0.8432`
- fine-tuned pre-trained base test accuracy: `0.8571`

This showed that transfer learning clearly outperformed the scratch-trained CNN for this task.

## Tools, Frameworks, and Libraries

This project uses:

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- TensorFlow / Keras
- PyTorch
- scikit-learn

## Reproducibility

The notebook was prepared with reproducibility in mind:

- random seed set to `42`
- outputs retained in notebook cells
- required plots saved with assignment-specified filenames
- model summaries included for built models

## How to Open and Run

1. Clone this repository.
2. Open `CNN_Lab_main.ipynb` in Jupyter Notebook, JupyterLab, or VS Code.
3. Run the cells in order if you want to reproduce outputs locally.
4. Make sure the required Python packages are installed before execution.

## Repository Notes

- The notebook is the main academic submission file.
- The figures in this repository are generated directly from notebook experiments.
- Helper development files may exist locally during experimentation, but the notebook and saved figures are the important final artifacts.

