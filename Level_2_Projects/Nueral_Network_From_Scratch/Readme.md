# Neural Network from Scratch for Handwritten Digit Classification

## Project Overview
This project implements a simple neural network from scratch using **NumPy** to classify handwritten digits from a MNIST-style dataset (`train.csv`). It demonstrates the fundamentals of neural networks without relying on deep learning frameworks such as TensorFlow or PyTorch.

### Features
- Data preprocessing and normalization
- Weight initialization
- Forward propagation using **ReLU** and **Softmax**
- Backward propagation and gradient computation
- Parameter updates via gradient descent
- One-hot encoding for multi-class classification
- Accuracy evaluation on training and development sets
- Visualization of sample predictions

## Dataset
The dataset consists of handwritten digit images stored in CSV format. Each row contains a label (0–9) followed by 784 pixel values (28x28 image flattened).  

- **Training set:** Remaining data after dev set extraction  
- **Development set:** First 1000 samples  

## Model Architecture
- Input layer: 784 neurons
- Hidden layer: 10 neurons, **ReLU** activation
- Output layer: 10 neurons, **Softmax** activation

## Results
- Training accuracy (approx.): 89.9%
- Development set accuracy: 90.3%
- Gradual improvement in accuracy observed across iterations
