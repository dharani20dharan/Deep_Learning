# IMDb Sentiment Analysis using RNN (PyTorch)

### Overview
A baseline Recurrent Neural Network (RNN) model for binary sentiment classification on the IMDb Movie Reviews dataset.  
The model aims to classify each review as either positive or negative.

---

### Model Summary
- Embedding Layer (64-dim)
- SimpleRNN (128 hidden units)
- Dense Output (Sigmoid)
- Loss: Binary Cross Entropy
- Optimizer: Adam

---

### Training Results
| Epoch | Loss | Accuracy |
|:--:|:--:|:--:|
| 1 | 0.6968 | 0.5019 |
| 2 | 0.6925 | 0.5212 |
| 3 | 0.6916 | 0.5237 |

**Test Accuracy:** ~57.9%

---

### Observations
- The model learns basic sentiment cues but underfits overall.
- Long-sequence dependencies cause accuracy stagnation.
- Suggested improvements: **LSTM/GRU**, **Dropout**, **Pretrained embeddings (GloVe)**.

---
