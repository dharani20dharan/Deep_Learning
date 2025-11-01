# CNN Model Variants Comparison (PyTorch)

## Overview
This project compares multiple Convolutional Neural Network (CNN) architectures on a dataset containing 1000 features. Each variant differs in the number of filters, kernel sizes, convolutional layers, and pooling types. The goal is to evaluate how these architectural changes affect model performance on a classification task.

## Dataset and Preprocessing
- The dataset consists of 1000 features and corresponding labels.
- Features are normalized using Min-Max scaling.
- Data is reshaped into 32×32×1 format (padded from 1000 to 1024 features) for CNN input.
- Split ratio: 80% training and 20% testing.

## Model Variants
Each model was built using different configurations:
- Filters: 16, 32, or 64  
- Kernel sizes: 3×3 or 5×5  
- Convolutional layers: 1–3  
- Pooling type: Max or Average

All models use ReLU activation, batch normalization, dropout, and a final softmax output layer.

## Training Details
- Optimizer: Adam  
- Loss Function: CrossEntropyLoss  
- Epochs: 30  
- Batch Size: 32  
- Early stopping based on validation loss

## Results Summary

| Model | Filters | Kernel | Conv Layers | Pooling | Train Acc | Val Acc | Test Acc |
|:------|:--------|:--------|:-------------|:----------|:-----------|:----------|:-----------|
| Variant_1 | 16 | 3 | 1 | max | 0.3719 | 0.3125 | 0.315 |
| Variant_2 | 16 | 5 | 1 | avg | 0.3516 | 0.3000 | 0.300 |
| Variant_3 | 32 | 3 | 2 | max | 0.3297 | 0.3500 | 0.300 |
| Variant_4 | 32 | 5 | 2 | avg | 0.4422 | 0.3000 | 0.315 |
| Variant_5 | 64 | 3 | 3 | max | 0.3688 | 0.3125 | 0.315 |
| Variant_6 | 64 | 5 | 3 | avg | 0.6219 | 0.3375 | 0.325 |

## Observations
- Increasing filters improved training accuracy but led to slight overfitting.
- Larger kernels (5×5) did not consistently improve validation accuracy.
- Max pooling provided slightly more stable performance than average pooling.
- Variant_6 achieved the highest training accuracy, though validation results remained moderate.

## Conclusion
Architectural depth and filter size influence model learning capacity but require careful tuning to balance accuracy and generalization. Further improvements may be achieved using regularization, data augmentation, and learning rate optimization.
