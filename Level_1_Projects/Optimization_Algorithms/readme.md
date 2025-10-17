# Optimizer Comparison Project

This project compares the performance of different optimizers on a classification task using a neural network. The goal is to observe how various optimization algorithms affect training speed, loss reduction, and final accuracy.

## Optimizers Tested

* SGD
* SGD with Momentum
* RMSprop
* Adam

## Observations

* SGD improved steadily but slowly.
* Momentum converged faster with better accuracy.
* RMSprop gave the best accuracy in this run.
* Adam performed well and is a strong default option.

## Requirements

* Python 3.8+
* PyTorch
* Matplotlib
* NumPy
* Jupyter Notebook

Install dependencies using:

```bash
pip install torch matplotlib numpy jupyter
```

## Results Summary

| Optimizer | Final Accuracy |
| --------- | -------------- |
| SGD       | ~0.79          |
| Momentum  | ~0.95          |
| RMSprop   | ~0.97          |
| Adam      | ~0.94          |

## License

This project is for educational and experimental purposes.
