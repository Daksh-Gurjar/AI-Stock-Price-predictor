# 🤖 Advanced AI Stock Price Predictor

A powerful, interactive stock price prediction tool built with multiple AI/ML models and real-time data fetching. Designed to run in Google Colab or any Jupyter Notebook environment.

---

## ✨ Features

- **Real-time data fetching** from Yahoo Finance for any stock ticker
- **Multiple AI/ML models** trained and compared side-by-side:
  - LSTM (Long Short-Term Memory) neural network
  - Random Forest
  - XGBoost
  - Ensemble (combination of all models)
- **51 advanced technical indicators** including moving averages, RSI, MACD, Bollinger Bands, and more
- **Future price predictions** with configurable forecast horizon
- **Comprehensive visualizations** — interactive dashboard saved as a PNG
- **Model persistence** — trained models are saved and can be reloaded
- Works for **any stock ticker** (e.g., `AAPL`, `TSLA`, `GOOGL`, `MSFT`)

---

## 📋 Prerequisites

- Python 3.8+
- [Google Colab](https://colab.research.google.com/) (recommended) or a local Jupyter Notebook environment

---

## 🚀 Getting Started

### Option 1: Run in Google Colab (Recommended)

1. Open [Google Colab](https://colab.research.google.com/).
2. Upload `AI_Stock_Price_Predictor.ipynb` or open it directly from GitHub.
3. Run the notebook cell — all dependencies are installed automatically.

### Option 2: Run Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Daksh-Gurjar/AI-Stock-Price-predictor.git
   cd AI-Stock-Price-predictor
   ```

2. **Install dependencies:**
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn xgboost tensorflow yfinance
   ```

3. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook AI_Stock_Price_Predictor.ipynb
   ```

4. **Run all cells** in the notebook.

---

## 🖥️ Usage

When you run the notebook, you will be prompted interactively:

1. **Enter a stock ticker symbol** (e.g., `AAPL`, `TSLA`, `GOOGL`):
   ```
   📈 Enter stock ticker symbol (e.g., AAPL, TSLA, GOOGL): AAPL
   ```

2. **Select a data period:**
   ```
   📅 Data period options:
     1. Last 1 year
     2. Last 2 years
     3. Last 3 years (Recommended)
     4. Last 5 years
     5. Custom
   ```

3. **Configure training parameters:**
   ```
   🎯 Training Configuration:
     Enter number of epochs (default 100): 20
     Enter forecast horizon in days (default 1): 1
   ```

The predictor will then:
- Fetch real-time data from Yahoo Finance
- Engineer 51 technical indicator features
- Train all three models (LSTM, Random Forest, XGBoost)
- Print a detailed report with performance metrics (RMSE, MAE, R², MAPE)
- Generate and save a visualization dashboard (e.g., `AAPL_analysis_dashboard.png`)

---

## 📊 Example Output

```
📄 STOCK PREDICTION REPORT - AAPL
======================================================================

📊 STOCK INFORMATION:
  • Ticker Symbol:   AAPL
  • Current Price:   $247.45
  • Total Return:    +13.20%
  • 52-Week High:    $258.10
  • 52-Week Low:     $172.00

🤖 MODEL PERFORMANCE:

  LSTM:    RMSE: $8.97 | MAE: $7.56 | R²: 0.3472 | MAPE: 3.13%
  RF:      RMSE: $6.41 | MAE: $5.36 | R²: 0.8324 | MAPE: 2.25%
  XGB:     RMSE: $6.10 | MAE: $4.96 | R²: 0.8482 | MAPE: 2.12%

🏆 BEST MODEL: XGB with R² = 0.8482
```

---

## 🧰 Tech Stack

| Library | Purpose |
|---|---|
| `yfinance` | Real-time stock data fetching |
| `numpy` / `pandas` | Data manipulation |
| `scikit-learn` | Random Forest, preprocessing, metrics |
| `xgboost` | XGBoost model |
| `tensorflow` / `keras` | LSTM neural network |
| `matplotlib` / `seaborn` | Visualizations |

---

## 📁 Project Structure

```
AI-Stock-Price-predictor/
├── AI_Stock_Price_Predictor.ipynb   # Main notebook
├── LICENSE                          # MIT License
└── README.md                        # Project documentation
```

> **Note:** A `saved_models/` directory is created automatically at runtime to store trained model files.

---

## ⚠️ Disclaimer

This project is for **educational and research purposes only**. Stock price predictions are inherently uncertain and should **not** be used as financial advice or as the sole basis for investment decisions.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
