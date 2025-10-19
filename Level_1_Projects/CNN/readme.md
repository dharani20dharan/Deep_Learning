# FashionMNIST Image Classification using CNNs (PyTorch)

This project implements a Convolutional Neural Network (CNN) to classify clothing images from the FashionMNIST dataset. The model is trained and evaluated to achieve strong accuracy in recognizing different clothing categories.

## Project Overview

- Load and preprocess the FashionMNIST dataset  
- Build a simple CNN from scratch using PyTorch  
- Train and validate the model  
- Evaluate performance using accuracy and confusion matrix  
- Visualize training and validation learning curves

## Dataset Information

- Image size: 28×28 grayscale  
- Number of classes: 10 clothing categories (e.g., T-shirt, trouser, coat)  
- Training images: 60,000  
- Test images: 10,000

## Model Training Results

| Epoch | Train Loss | Train Acc | Val Loss | Val Acc |
|-------|------------|-----------|----------|---------|
| 1     | 0.5043     | 82.22%    | 0.3959   | 85.79%  |
| 5     | 0.2482     | 91.18%    | 0.2685   | 90.72%  |
| 10    | 0.1888     | 93.25%    | 0.2655   | 90.56%  |
| 15    | 0.1526     | 94.43%    | 0.2594   | 91.22%  |
| 20    | 0.1299     | 95.21%    | 0.2730   | 91.29%  |

**Final Validation Accuracy:** 91.29%  
**Final Training Accuracy:** 95.21%

## Key Steps

1. Download and normalize the FashionMNIST dataset  
2. Define a CNN architecture with convolution, pooling, and fully connected layers  
3. Train the model for 20 epochs with cross-entropy loss and Adam optimizer  
4. Evaluate the model on validation and test sets  
5. Plot training and validation curves to monitor performance

## Requirements

- Python 3.8+  
- PyTorch  
- torchvision  
- matplotlib  
- scikit-learn
