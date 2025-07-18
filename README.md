# 📊 Flask Stock Market App with jugaad-data

This is a simple Flask application integrated with [`jugaad-data`](https://pypi.org/project/jugaad-data/) to fetch and process live stock data from NSE (National Stock Exchange, India). The project uses specific versions of Flask and Werkzeug to maintain compatibility.

# GrowUp Virtual Stock Simulator

GrowUp is a virtual stock market simulator that allows users to practice trading stocks without risking real money. It's an educational platform designed to help beginners learn about stock market investing in a risk-free environment.

## Key Features of GrowUp

1. **Virtual Portfolio**: Start with a predefined amount of virtual currency to build your investment portfolio.

2. **Real Market Data**: The simulator uses real-time market data from the National Stock Exchange (NSE) of India, providing an authentic trading experience.

3. **Trading Experience**: Users can buy and sell stocks, track performance, and learn about market movements without financial risk.

4. **Performance Analytics**: Track your investment performance with detailed reports, charts, and comparisons against market benchmarks.

5. **Learning Resources**: Access educational content about investing strategies, market analysis, and financial literacy.

6. **Social Features**: Compare performance with friends or other users, participate in trading competitions, and share insights.

## Educational Benefits

- **Risk-Free Learning**: Make mistakes and learn investing principles without losing real money.
- **Market Familiarity**: Become familiar with stock symbols, order types, and market terminology.
- **Strategy Testing**: Experiment with various investment strategies to see what works best.
- **Confidence Building**: Gain confidence before transitioning to real market investing.

## Target Audience

- Students learning about finance and investing
- New investors wanting to practice before using real funds
- Finance educators teaching practical market skills
- Anyone interested in understanding stock markets without financial commitment

GrowUp serves as a bridge between theoretical knowledge about stock markets and practical application, making it an ideal tool for financial education and skills development in investment management.

## 🛠️ Tech Stack

- **Backend**: NodeJs, ExpressJs and FastAPI (Python web framework)
- **Data Processing**: jugaad-data, pandas
- **Frontend**: HTML, CSS, JavaScript
- **Database**: MongoDB 
- **Other**: Websocket, JWT 
---

## ⚙️ Setup & Installation

Follow the steps below to set up the project from scratch:

### ✅ 1. Create and Activate Virtual Environment

**Windows:**
```bash
python -m venv venv
.\venv\Scripts\activate
pip install -r requirements.txt

## 🚀 Running the App

```bash
python combined_app.py
```

## 📚 Dependencies

- **Flask** – Web application framework
- **Werkzeug** – WSGI utility library used by Flask
- **jugaad-data** – For fetching live market data from NSE
- **pandas** – Data analysis and manipulation
