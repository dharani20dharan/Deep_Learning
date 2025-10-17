# SLP vs MLP Regression using PyTorch

This project implements **Single Layer Perceptron (SLP)** and **Multi Layer Perceptron (MLP)** models for regression on a synthetic dataset using PyTorch. The performance of both models is compared using **Mean Absolute Error (MAE)**, **Mean Squared Error (MSE)**, and **R² Score**.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Models](#models)
- [Results](#results)
- [Insights](#insights)
- [Conclusion](#conclusion)
- [Requirements](#requirements)

## Project Overview
The goal of this project is to compare the performance of a simple linear model (SLP) with a more complex non-linear model (MLP) for regression tasks. The project demonstrates the importance of model selection based on dataset complexity.

## Dataset
A synthetic dataset is generated with non-linear relationships between input features and target values. The dataset is split into training and testing sets for model evaluation.

## Models
### Single Layer Perceptron (SLP)
- Linear model with one layer.
- Suitable for datasets with linear relationships.

### Multi Layer Perceptron (MLP)
- Deep neural network with multiple layers.
- Uses non-linear activation functions (ReLU).
- Includes dropout layers to prevent overfitting.
- Capable of capturing complex non-linear patterns.

## Results

| Model | MAE   | MSE    | R²     |
|-------|-------|--------|--------|
| SLP   | 15.24 | 359.92 | 0.062  |
| MLP   | 8.18  | 108.81 | 0.716  |

## Insights
- **SLP** performs poorly on non-linear data due to its linear nature.
- **MLP** captures non-linear patterns effectively, achieving significantly lower error and higher R² scores.
- Dropout layers in MLP improve generalization and help prevent overfitting.
- Choosing the right architecture is critical for achieving good performance on complex datasets.

## Conclusion
For regression tasks with non-linear relationships, **MLP is the preferred model**, while SLP is only suitable for simple linear patterns.

## Requirements
- Python 3.8+
- PyTorch
- NumPy
- scikit-learn
- matplotlib (optional, for visualization)


