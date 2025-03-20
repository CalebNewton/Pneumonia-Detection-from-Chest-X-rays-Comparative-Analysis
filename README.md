# Pneumonia-Detection-from-Chest-X-rays-Comparative-Analysis
## Overview
This project presents a deep learning-based solution for the detection of pneumonia from chest X-ray images. It involves the development of a custom Convolutional Neural Network (CNN) model and a comparative analysis with four popular pretrained models: MobileNetV2, ResNet50, DenseNet201, and VGG-19. The objective is to explore the performance of these models while also investigating the effects of hyperparameter tuning (e.g., convolutional layers and optimizers) on the accuracy of pneumonia detection.

## Motivation
Pneumonia is a leading cause of death in children, especially in under-resourced regions. Accurate and early detection can be life-saving. In this study, we aim to improve pneumonia detection using AI by:
 * Building a custom CNN architecture from scratch.
 * Analyzing the impact of different hyperparameters on model performance.
 * Comparing the custom model against industry-standard pretrained networks.

## Dataset
The dataset used is the publicly available chest X-ray dataset by Kermany et al. (2018), consisting of 5,856 X-ray images categorized into "Normal" and "Pneumonia" classes.
   * Training samples: 5,232
   * Test samples: 624

## Methodology
### 1. Custom CNN Model
   * Four convolutional layers.
   * ReLU activation and max pooling.
   * Dense layers with dropout regularization.
   * Sigmoid activation for binary classification.

### 2. Hyperparameter Tuning
   * Compared models with 3, 5, and 6 convolutional layers.
   * Tested optimizers: Adam (proposed), SGD, RMSprop, Adagrad.

### 3. Pretrained Models
   * MobileNetV2
   * ResNet50
   * DenseNet201
   * VGG-19

## Results
Proposed CNN Model: Achieved 91% accuracy with 90% recall, precision, and F1-score.
Best Pretrained Model: VGG-19 achieved 93% precision and matched 91% accuracy with ResNet50.
Adam optimizer and four convolutional layers produced the best results among hyperparameter variations.

