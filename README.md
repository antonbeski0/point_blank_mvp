# POINT.BLANK
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

**Point.Blank** — an advanced Streamlit application for stock market data visualization, technical analysis, news aggregation, and machine learning–based forecasting (Prophet, ARIMA, Random Forest, LSTM).  
It is designed for **interactive exploration**, **data export**, and **AI-driven forecasting** — all within a clean, intuitive interface.

---

## 📘 Table of Contents
- [✨ Key Features](#-key-features)
- [🖼️ Screenshots](#️-screenshots)
- [⚙️ Requirements](#️-requirements)
- [🚀 Installation](#-installation)
- [⚡ Quick Start](#-quick-start)
- [🔧 Configuration & Options](#-configuration--options)
- [🧠 Forecasting Models](#-forecasting-models)
- [🧩 Internals & Architecture](#-internals--architecture)
- [🤝 Contributing](#-contributing)
- [📜 License](#-license)
- [👤 Author & Contact](#-author--contact)
- [⚠️ Disclaimer](#️-disclaimer)

---

##  Key Features
- **Live Market Data** — Fetch historical data from Yahoo Finance (`yfinance`) with validation and retry handling.  
- **Dynamic Charts** — Plotly-powered interactive charts with SMA, MACD, RSI, Bollinger Bands, ATR, and more.  
- **AI Insights** — Compute technical analysis summaries, overall signal strength, and price trends.  
- **News Aggregation** — Automatically collects and filters financial news via RSS feeds with deduplication.  
- **ML Forecasting** — Integrates multiple forecasting engines:
  - **Prophet** — regression-based forecasting with additional regressors.  
  - **ARIMA** — automated order selection and stationarity checks.  
  - **Random Forest** — feature-rich time series regression.  
  - **LSTM (TensorFlow)** — deep-learning sequence forecasting for longer datasets.  
- **Data Export** — Export analysis results and news to CSV or JSON.  

---

##  Screenshots
<p align="center">
  <img width="744" height="496" alt="App Screenshot 1" src="https://github.com/user-attachments/assets/557f11f6-f580-4480-9594-bd7c53370c4e" />
  <img width="508" height="304" alt="App Screenshot 2" src="https://github.com/user-attachments/assets/8cc0fa52-7824-4ffd-bb4e-72452b6a081c" />
</p>

---

##  Requirements

### Core Dependencies
```bash
Python >= 3.9
streamlit
yfinance
pandas
numpy
plotly
streamlit-plotly-events
feedparser
pytz
requests
```

### Optional (for forecasting)
```bash
prophet
statsmodels
pmdarima
scikit-learn
tensorflow
```

---

##  Installation

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/antonbeski0/point_blank_mvp
cd point_blank.stream
```

### 2️⃣ Create a Virtual Environment (Recommended)
```bash
# Windows
python -m venv .venv
.venv\Scripts\activate

# macOS / Linux
python3 -m venv .venv
source .venv/bin/activate
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```
Or manually:
```bash
pip install streamlit yfinance pandas numpy plotly streamlit-plotly-events feedparser pytz requests
```

### 4️⃣ (Optional) Install ML Libraries
```bash
# All ML packages
pip install prophet statsmodels pmdarima scikit-learn tensorflow
```

---

## ⚡ Quick Start
Run the app with:
```bash
streamlit run point_blank.py
```
Then open your browser at **http://localhost:8501**.

---

## 🔧 Configuration & Options
- **Ticker Validation** — Prevents invalid queries.  
- **Auto-Detection** — Checks available ML libraries for advanced forecasting.  
- **Export Options** — Export charts, analysis, and news feeds in CSV or JSON formats.  

---

##  Forecasting Models
- **Prophet** — Regression-based time series forecasting.  
- **ARIMA** — Stationarity tests with auto order selection.  
- **Random Forest** — Ensemble learning for short-term predictions.  
- **LSTM (TensorFlow)** — Sequence-to-sequence neural forecasting.  

---

##  Internals & Architecture
| Function | Purpose |
|-----------|----------|
| `fetch_yahoo_data()` | Fetches and validates market data. |
| `compute_indicators()` | Calculates key indicators (SMA, MACD, RSI, etc.). |
| `generate_technical_analysis()` | Summarizes technical insights and signals. |

---

##  Contributing
1. Fork the repository  
2. Create a feature branch  
   ```bash
   git checkout -b feat/your-feature
   ```  
3. Commit and push your changes  
4. Submit a Pull Request  

---

##  License
This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

##  Author & Contact
**Anton Beski M** 
 antbsk0@gmail.com
 For support or feedback — please open an **Issue** or **Pull Request** on GitHub.

---

## ⚠️ Disclaimer
> **Point.Blank** provides financial data and forecasts **for educational purposes only**.  
> It does **not** constitute financial, trading, or investment advice.
