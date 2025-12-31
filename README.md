# 📈 Stock Predictor

A comprehensive stock analysis platform integrating **Machine Learning forecasting**, **Technical Analysis**, and **Sentiment Analysis** to provide data-driven market insights.



---

## 🚀 Key Features

### 🤖 AI Models & Algorithms
The platform utilizes an ensemble approach to time-series forecasting:
* **Deep Learning:** LSTM, GRU, and CNN-LSTM (via TensorFlow.js) for complex pattern recognition.
* **Statistical Models:** ARIMA and Prophet-Lite for trend and seasonality detection.
* **Traditional ML:** Linear Regression and Exponential Moving Averages (EMA).
* **Ensemble Engine:** A weighted combination of all models for optimized prediction accuracy.



### 📊 Technical Analysis & Patterns
* **Indicators:** Moving Averages (20/50/200-day), RSI, MACD, and Bollinger Bands.
* **Pattern Detection:** Automatic identification of trendlines, wedges, triangles, channels, double tops/bottoms, and head & shoulders patterns.
* **Flexible Timeframes:** Analysis across 5m, 15m, 1H, 1D, 1W, and 1M intervals.

### 📰 News Sentiment Analysis
A custom rule-based NLP engine optimized for financial markets:
* **Negation & Intensity:** Handles "not good" or "extremely bullish" via negation flips and intensity modifiers.
* **Financial Lexicon:** 100+ domain-specific terms (e.g., "earnings beat", "missed estimates").
* **Pattern Matching:** Detects and weighs percentage gains/losses mentioned in headlines.

### 💡 Market Insights
* **Trading Signals:** Automated Buy/Sell recommendations based on indicator crossovers.
* **Volume Analysis:** Identification of unusual trading activity and "smart money" moves.
* **Momentum Tracking:** Evaluation of price action strength.

---

## 🛠 Prerequisites

Before installation, ensure you have the following:
* **Node.js 18+** installed.
* **NewsAPI Key:** Get one at [newsapi.org](https://newsapi.org/).
* **Alpha Vantage API Key:** Get one at [alphavantage.co](https://www.alphavantage.co/).
* **MASSIVE API Key:** (Optional) For company logos and metadata.

---

## ⚙️ Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/sankeer28/stock-predictor.git](https://github.com/sankeer28/stock-predictor.git)
    cd stock-predictor
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Environment Setup:**
    Create a `.env.local` file in the root directory:
    ```bash
    cp .env.local.example .env.local
    ```
    Add your API keys to the `.env.local` file:
    ```env
    NEWS_API_KEY=your_api_key_here
    ALPHA_VANTAGE_API_KEY=your_api_key_here
    ```

4.  **Run Development Server:**
    ```bash
    npm run dev
    ```
    Visit [http://localhost:3000](http://localhost:3000) to view the app.

---

## 🤝 Contributing

Contributions make the open-source community an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.
