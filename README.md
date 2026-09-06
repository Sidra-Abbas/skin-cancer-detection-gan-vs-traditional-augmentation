Skin Cancer Detection Using Traditional Data Augmentation and GANs
Project Overview
This repository contains the code implementation for a thesis study on automated skin cancer lesion classification. The research evaluates model performance across three benchmark dermatoscopic datasets: HAM10000, HIBA, and ProvenAI.

The study investigates baseline classification performance using Traditional Data Augmentation techniques (rotations, flips, scaling, zooming, and color adjustments) compared against synthetic data generation using Generative Adversarial Networks (GANs) to handle dataset class imbalance.

Evaluated Models
The experiments incorporate four deep learning architectures across the datasets:

4Block-Progressive-CNN

ResNet50

ResNet101

EfficientNet-B0
Experimental Workflow
Preprocessing: Image resolution standardization, intensity normalization, and stratified train/validation/test splitting.

Traditional Augmentation: Spatial transformations (flips, rotations, scaling) to improve feature invariance and reduce overfitting.

GAN Synthetic Augmentation: Training generative models to produce artificial lesion samples for underrepresented minority classes.

Classification Training: Executing model training across 4Block-Progressive-CNN, ResNet50, ResNet101, and EfficientNet-B0 architectures.

Evaluation: Assessing performance using Accuracy, Precision, Recall, F1-Score, and AUC-ROC metrics.
Installation & Prerequisites
To run the notebooks, install the required dependencies:

"pip install numpy pandas matplotlib scikit-learn tensorflow torch torchvision albumentations"
