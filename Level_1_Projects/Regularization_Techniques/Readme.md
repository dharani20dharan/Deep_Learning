# Neural Network Regularization Techniques

This project demonstrates the effect of various regularization techniques on a binary classification problem using PyTorch. It explores how models generalize to unseen data when different regularization methods are applied.

---

## Project Overview

Neural networks are prone to overfitting, especially with small datasets or complex architectures. Regularization techniques help prevent overfitting and improve generalization. In this project, we implemented a feedforward neural network and experimented with:

1. **Base Model** – Standard feedforward network without regularization.  
2. **Dropout Model** – Incorporates dropout layers to randomly deactivate neurons during training.  
3. **L2-Regularized Model** – Applies L2 weight decay to penalize large weights.  
4. **L1-Regularized Model** – Applies L1 regularization to encourage sparsity in the network weights.  

---

## Dataset

- **File:** `regularizer_lab_classification_dataset.csv`  
- **Description:** Binary classification dataset.  
- **Preprocessing:** Features are standardized using `StandardScaler`.  
- **Split:** Training (80%) and validation (20%).

---

## Implementation

- Framework: PyTorch  
- Loss Function: Binary Cross-Entropy (`BCELoss`)  
- Optimizer: Adam  
- Training: 50 epochs with batch size 32  
- Regularization:
  - Dropout rate: 0.5
  - L2 weight decay: 0.01
  - L1 lambda: 0.001

---

## Key Observations

- **Base Model:** Fast training loss reduction but validation loss plateaus, indicating overfitting.  
- **Dropout Model:** Slower training loss reduction but better generalization; reduces overfitting effectively.  
- **L2-Regularized Model:** Maintains a stable balance between training and validation loss.  
- **L1-Regularized Model:** Promotes sparsity in weights, slightly higher training loss initially, but improved generalization.

**Conclusion:**  
Regularization techniques such as Dropout, L1, and L2 help mitigate overfitting and improve the model's performance on unseen data. Selecting the right regularization method is essential for achieving optimal generalization.

---
