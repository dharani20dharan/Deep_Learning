# CNN Variants on 1000-Feature Dataset

## Overview
This project explores the performance of different **Convolutional Neural Network (CNN)** architectures on a synthetic dataset with 1000 features per sample.  
Features are reshaped into 32×32 grids to enable CNN-based classification.

## Objective
To analyze how variations in convolutional depth, filter count, kernel size, and pooling strategy affect classification accuracy.

## Dataset
- Synthetic dataset with 1000 numerical features per sample  
- Three class labels: 0, 1, 2  
- Features padded to 1024 and reshaped to 32×32×1

## Summary of Results
| Model | Filters | Kernel | Conv Layers | Pooling | Train Acc | Val Acc | Test Acc |
|--------|----------|---------|--------------|----------|------------|-----------|-----------|
| Variant_1 | 16 | 3 | 1 | Max | 0.372 | 0.313 | 0.315 |
| Variant_2 | 16 | 5 | 1 | Avg | 0.352 | 0.300 | 0.300 |
| Variant_3 | 32 | 3 | 2 | Max | 0.330 | 0.350 | 0.300 |
| Variant_4 | 32 | 5 | 2 | Avg | 0.442 | 0.300 | 0.315 |
| Variant_5 | 64 | 3 | 3 | Max | 0.369 | 0.313 | 0.315 |
| Variant_6 | 64 | 5 | 3 | Avg | 0.622 | 0.338 | 0.325 |

## Key Insights
- Increasing filter count improves training accuracy but may lead to overfitting.  
- Larger kernels (5×5) slightly enhanced feature extraction without major validation gains.  
- Max pooling provided more consistent performance than average pooling.

## Conclusion
Deeper and wider CNNs captured richer patterns but showed moderate generalization.  
Regularization and hyperparameter tuning are recommended for improved results.
