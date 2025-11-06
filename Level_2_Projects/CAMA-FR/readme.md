# CAMA-FR: Channel-Attention Model Adaptation for Face Recognition

A deep learning project exploring **Adaptive Feature Fusion (AFF)** and **Knowledge Distillation (KD)** in ResNet-based architectures for face verification tasks.

## Overview
This work investigates how attention-based adaptation and teacher–student knowledge transfer influence face representation quality.  
Experiments were conducted on the **LFW** dataset, comparing baseline CNNs with AFF-enhanced variants.

## Features
- Implementation of **ResNet Student–Teacher Framework**
- Integration of **Adaptive Feature Fusion (AFF)**
- **Knowledge Distillation (KD)** with cosine similarity loss
- Evaluation using **ROC**, **AUC**, and **t-SNE visualization**

## Results Summary
| Model | AUC |
|--------|------|
| Baseline | 0.6368 |
| AFF | 0.6034 |

## Key Insights

- Channel attention enhances intra-class compactness but may reduce generalization if not properly regularized.

- Knowledge distillation helps transfer robust features from the teacher model.

- Further improvements could include margin-based losses or data augmentation.