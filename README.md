# 📈 Tesla Stock Price Prediction using LSTM

This project uses a Long Short-Term Memory (LSTM) neural network to predict Tesla's stock closing prices. It leverages deep learning techniques for time series forecasting, using historical stock data.

---

## 🚀 Project Overview

- 🔍 **Goal**: Predict the next day's closing price of Tesla stock using the last 60 days of prices.
- ⚙️ **Model**: LSTM Neural Network
- 📊 **Input**: Past 60 days of closing prices
- 📈 **Output**: Next day's predicted closing price

---

## 🧰 Technologies & Libraries

- **Python**
- [Pandas](https://pandas.pydata.org/) – Data processing
- [NumPy](https://numpy.org/) – Numerical operations
- [Matplotlib](https://matplotlib.org/) – Visualization
- [Scikit-learn](https://scikit-learn.org/) – Data scaling
- [TensorFlow/Keras](https://www.tensorflow.org/) – Deep learning model

---

## 🧠 Model Architecture

```text
Input → LSTM (50 units, return_sequences=True)
      → LSTM (50 units) 
      → Dense (25) 
      → Dense (1) → Predicted closing price
```

- Optimizer: Adam  
- Loss Function: Mean Squared Error  
- Epochs: 1 (can be increased)

---

## 📁 Files in This Repo

| File | Description |
|------|-------------|
| `tesla-stock-prediction.ipynb` | Jupyter notebook with full data preprocessing, LSTM model, prediction, and visualization |
| `tesla_stock_data_2000_2025.csv` | Tesla historical stock price dataset (from Yahoo Finance) |
| `README.md` | Project overview and instructions |

---

## 📉 Example Results

The chart below shows the actual vs predicted closing prices for the validation set:

> *(Add this plot to your repo as `result.png` and embed below)*

![Model Prediction](result.png)

---

## 🔄 How It Works

1. Load and normalize Tesla stock closing prices
2. Create sliding windows of 60-day sequences
3. Train an LSTM model on the training data
4. Predict on test data
5. Visualize the predictions vs actual values
6. Predict the next day's closing price using the last 60 days

---

## 📦 How to Run

1. Clone the repo:

```bash
git clone https://github.com/your-username/tesla-stock-prediction.git
cd tesla-stock-prediction
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Open the notebook:

```bash
jupyter notebook tesla-stock-prediction.ipynb
```

---

## ✅ Future Improvements

- Add more features (Open, High, Low, Volume)
- Use additional models (GRU, Transformer)
- Increase epochs, tune hyperparameters
- Add performance metrics like RMSE, MAE

---

## 📬 Contact

If you liked the project or want to collaborate, feel free to connect:

- GitHub: [@dominator1920](https://github.com/dominator1920)
- LinkedIn: [Pranay Kshitiz](https://linkedin.com/in/pranay-kshitiz)

---

## 📜 License

This project is open-source and free to use under the [MIT License](LICENSE).
