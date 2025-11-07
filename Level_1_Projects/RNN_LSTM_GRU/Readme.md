#  Sentiment Analysis using RNN, LSTM, and GRU

This project implements **sentiment classification** on the Amazon Reviews dataset using three different Recurrent Neural Network architectures — **SimpleRNN**, **LSTM**, and **GRU** — to analyze text sequences and determine whether a review is positive or negative.

---

##  Dataset
- **Source:** `archive/Reviews.csv`  
- **Columns Used:** `Text`, `Score`  
- **Processing:**
  - Neutral reviews (`Score = 3`) are removed  
  - Positive sentiment: `Score ≥ 4` → 1  
  - Negative sentiment: `Score ≤ 2` → 0  

---

##  Project Workflow
1. **Data Preprocessing**
   - Clean and select relevant columns  
   - Tokenize and pad sequences (max 100 words per review)  

2. **Model Construction**
   - **SimpleRNN**: Basic recurrent network for sequence processing  
   - **LSTM**: Long Short-Term Memory for long-range dependencies  
   - **GRU**: Gated Recurrent Unit for efficient sequence learning  

3. **Training & Evaluation**
   - Train for 5 epochs each  
   - Evaluate accuracy on test set  
   - Visualize performance  

---

##  Model Performance
| Model     | Test Accuracy |
|------------|---------------|
| SimpleRNN | **84.18%**    |
| LSTM      | **95.88%**    |
| GRU       | **95.77%**    |

---

##  Conclusion

LSTM and GRU outperform the basic RNN, achieving over 95% accuracy.

They effectively capture long-term dependencies in text sequences.

The experiment highlights the power of advanced recurrent architectures for sentiment analysis.

