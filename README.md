# Deep Learning Projects Collection

This repository houses a structured collection of Deep Learning projects, organized by complexity and domain. The projects range from foundational neural network implementations to advanced applications in computer vision and natural language processing.

## 📂 Project Structure

The repository is divided into levels to guide learners and researchers through a progressive deep learning journey.

### 🔹 [Level 1 Projects](./Level_1_Projects) (Foundational)
These projects focus on core deep learning concepts and standard architectures.

- **[CNN](./Level_1_Projects/CNN)**: Convolutional Neural Networks for image classification.
- **[CNN_Variants](./Level_1_Projects/CNN_Variants)**: Exploration of different CNN standard architectures.
- **[Face_Recognition](./Level_1_Projects/Face_Recognition)**: Implementation of face recognition systems.
- **[Optimization_Algorithms](./Level_1_Projects/Optimization_Algorithms)**: Comparative analysis of optimizers (SGD, Adam, RMSprop).
- **[Regularization_Techniques](./Level_1_Projects/Regularization_Techniques)**: Techniques to prevent overfitting (Dropout, L1/L2).
- **[RNN](./Level_1_Projects/RNN)**: Recurrent Neural Networks for sequential data.
- **[RNN_LSTM_GRU](./Level_1_Projects/RNN_LSTM_GRU)**: Advanced sequence modeling with LSTMs and GRUs for sentiment analysis.
- **[SLP_MLP](./Level_1_Projects/SLP_MLP)**: Single vs. Multi-Layer Perceptrons for regression tasks.

### 🔸 [Level 2 Projects](./Level_2_Projects) (Intermediate/Advanced)
These projects involve more complex implementations, custom architectures, and scratch-built models.

- **[CAMA-FR](./Level_2_Projects/CAMA-FR)**: **Channel-Attention Model Adaptation for Face Recognition**. Investigates Adaptive Feature Fusion (AFF) and Knowledge Distillation.
- **[Nueral_Network_From_Scratch](./Level_2_Projects/Nueral_Network_From_Scratch)**: A complete implementation of a neural network using only **NumPy**, allowing for a deep understanding of backpropagation and gradient descent.

### ▫️ [Level 3 Projects](./Level_3_Projects)
*Reserved for future advanced research and large-scale model implementations.*

---

## 🛠️ Common Requirements
Most projects in this repository require the following dependencies:

- **Python 3.8+**
- **PyTorch** (Core Deep Learning Framework)
- **NumPy** & **Pandas** (Data Manipulation)
- **Matplotlib** & **Seaborn** (Visualization)
- **Jupyter Notebook** (Interactive Development)

Install the base requirements using:
```bash
pip install torch torchvision numpy pandas matplotlib jupyter
```
*Note: Specific projects may have unique `requirements.txt` or dependencies listed in their respective READMEs.*

## 🚀 Getting Started
1. Clone the repository.
2. Navigate to a project folder of interest (e.g., `cd Level_1_Projects/CNN`).
3. Follow the instructions in the project's `README.md` to run the notebooks or scripts.

---
**Author**: Dharanidharan  
**Purpose**: Educational & Research
