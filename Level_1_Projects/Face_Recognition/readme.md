#  Face Recognition using CNN, MobileNet, and ResNet

##  Project Overview
This project implements and compares three deep learning architectures — a **Baseline CNN**, **MobileNetV2**, and **ResNet50** — for image classification on a custom face recognition dataset located in the `archive/` folder.  
It follows a 3-hour lab structure designed for hands-on understanding of dataset preparation, model building, transfer learning, and performance analysis using **PyTorch**.

---



##  Models Implemented

| Model | Description | Pretrained | Notes |
|--------|--------------|------------|--------|
| **Baseline CNN** | Simple custom CNN built from scratch | ❌ No | Used as performance reference |
| **MobileNetV2** | Lightweight model optimized for mobile devices | ✅ Yes | Fast and efficient transfer learning |
| **ResNet50** | Deep residual network for robust feature extraction | ✅ Yes | High performance, deeper architecture |

---

##  Final Results Summary

| Model | Best Val Accuracy | Training Time | Remarks |
|--------|--------------------|----------------|-----------|
| **Baseline CNN** | 74.36% | 3.78 min | Fast but less accurate |
| **MobileNetV2** | 82.76% | 11.99 min | Best generalization |
| **ResNet50** | 82.92% | 11.00 min | Stable and consistent |

---

##  Visualizations
- Accuracy and loss curves for training and validation sets.
- Comparative bar plots for model performance.

---

##  Tech Stack
- **Framework:** PyTorch  
- **Language:** Python  
- **Libraries:** torchvision, matplotlib, numpy, tqdm  
- **Dataset Format:** Image folders (`train/`, `test/`) inside `archive/`

---

## Conclusion

MobileNetV2 and ResNet50 outperform the baseline CNN significantly.

ResNet50 offers slightly higher accuracy, while MobileNetV2 is more efficient and lightweight.

For deployment, MobileNetV2 provides the best trade-off between accuracy and computation cost.