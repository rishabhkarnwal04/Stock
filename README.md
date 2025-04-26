# 📈 Stock Market Prediction and Sentiment Analysis System

An **end-to-end stock market prediction web application** built using **Streamlit**.  
It integrates **real-time stock data**, **advanced machine learning models**, **sentiment analysis on news**, and **beautiful interactive visualizations** — all in one platform.

---

By - Rishabh Karnwal

---

## 🚀 Features

✅ **Sector & Stock Selection**  
&nbsp;&nbsp;&nbsp;&nbsp;→ Choose Indian stocks categorized by sector (IT, Banking, Pharma, Energy).

✅ **Advanced Machine Learning Models**  
&nbsp;&nbsp;&nbsp;&nbsp;→ Predict stock movement using:
- Random Forest Classifier
- LightGBM Classifier
- CatBoost Classifier

✅ **Dynamic Visualizations**  
&nbsp;&nbsp;&nbsp;&nbsp;→ Multiple chart options:
- Candlestick Chart
- Moving Averages (MA20, MA50)
- Trading Volume Chart
- RSI (Relative Strength Index)

✅ **Real-Time News Sentiment Analysis**  
&nbsp;&nbsp;&nbsp;&nbsp;→ Fetch latest news headlines for the selected stock.  
&nbsp;&nbsp;&nbsp;&nbsp;→ Sentiment classification using **TextBlob** (Positive / Neutral / Negative).  
&nbsp;&nbsp;&nbsp;&nbsp;→ Visually highlighted.

✅ **Prediction Accuracy Display**  
&nbsp;&nbsp;&nbsp;&nbsp;→ Shows model’s prediction accuracy in percentage.

✅ **Predicted vs Actual Graph**  
&nbsp;&nbsp;&nbsp;&nbsp;→ Visual comparison of predicted labels vs actual future stock movement.

✅ **Advanced Settings** via Sidebar  
&nbsp;&nbsp;&nbsp;&nbsp;→ Change train-test split ratio, number of news articles, toggle graphs, models, etc.

✅ **Real-time Updates**  
&nbsp;&nbsp;&nbsp;&nbsp;→ Refresh stock data and sentiment analysis every few minutes.

✅ **User-Friendly and Fully Responsive UI**  
&nbsp;&nbsp;&nbsp;&nbsp;→ Designed with a clean, dark-themed Plotly UI and Streamlit sidebar controls.

---

## 🛠️ Technology Stack

| Technology | Purpose |
|:-----------|:--------|
| **Streamlit** | Building the web application |
| **Yahoo Finance API (yfinance)** | Real-time stock price and historical data |
| **NewsAPI** | Fetching live news articles |
| **TextBlob** | Sentiment analysis |
| **Scikit-learn** | Machine learning (train-test split, metrics, models) |
| **LightGBM** | Gradient boosting model |
| **CatBoost** | Advanced gradient boosting model optimized for categorical features |
| **Plotly** | Interactive graphs (candlestick, volume, RSI) |
| **Matplotlib** | Actual vs Predicted comparison plots |
| **Pandas** | Data manipulation |
| **NumPy** | Numerical operations |

---

## ⚙️ Installation and Setup

1. **Clone the Repository**  
```bash
git clone https://github.com/rishabhkarnwal04/Stock.git
cd stock
```

2. **Install Python Packages**  
```bash
pip install -r requirements.txt
python -m textblob.download_corpora
```

3. **Insert Your News API Key**  
In `stock.py`, replace:
```python
newsapi = NewsApiClient(api_key='YOUR_NEWSAPI_KEY')
```
with your **valid NewsAPI key**.

4. **Run the Streamlit App**  
```bash
streamlit run stock.py
```

---

## 🔑 Getting a Free NewsAPI Key

- Go to [https://newsapi.org/](https://newsapi.org/)
- Create an account (free)
- Generate your API Key
- Paste it into `stock.py`

---

## 🧪 How It Works

- **Load Historical Stock Data** from Yahoo Finance.
- **Feature Engineering**: Create features like Open-Close, High-Low.
- **Train ML Models**: Random Forest, LightGBM, and CatBoost using train-test split.
- **Make Predictions** on stock movement (up/down) for next time step.
- **Visualize Performance**: Model accuracy + predicted vs actual charts.
- **Fetch Real-Time News** and analyze headline sentiment.
- **Interactive Dashboard** for exploring all metrics and graphs dynamically.

---

## 💬 Future Improvements

- Add **LSTM** deep learning models for price prediction.
- Add **AutoML** model selection for best accuracy.
- Deploy on **Streamlit Cloud**, **AWS EC2**, or **Heroku**.
- Add **multi-stock portfolio prediction**.

---

## 📢 Important Notice

> This project is strictly for **educational purposes** and **should not be considered as financial advice**.  
> Stock market investments are subject to market risks. Please consult a licensed financial advisor.

---

## 🙌 Acknowledgements

- [Yahoo Finance](https://finance.yahoo.com/) for stock data
- [NewsAPI](https://newsapi.org/) for news headlines
- [TextBlob](https://textblob.readthedocs.io/en/dev/) for sentiment analysis
- [Streamlit](https://streamlit.io/) for UI framework

---

# ✨ Thank You for Checking Out This Project! ✨
