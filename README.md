# 📈 GrowwUp – Virtual Stock Market Simulator

**GrowwUp** is a real-time, beginner-friendly virtual stock trading simulator that allows users to understand the basics of the stock market without any financial risk. Designed as an experiential platform, it uses live NSE stock data, simulates buying/selling behavior, and provides portfolio tracking with personalized analysis.

---

## 🚀 Inspiration

As someone who started trading in my second year, I personally experienced the steep learning curve and confusion around basic market terminologies and trading strategies. GrowwUp is built to solve that gap — giving users a risk-free, real-world learning experience in the world of stock markets.

---

## 🎯 Features

- 📊 **Live NSE Stock Data** – Integrated using `nse-jugaad-data` (no paid API required)
- 🔁 **Real-Time Updates** – WebSocket-powered live price streaming
- 🚀 **Asynchronous FastAPI Backend** – Built with high-performance async I/O
- 🧠 **Portfolio Summary & Analyzer** – Get insights on portfolio performance and suggestions
- 🔄 **Order Management** – Simulate buy/sell operations with real-time timestamps
- ⚡ **TTL Cache** – Efficient caching of stock data to reduce latency and API load
- 🔐 **User Authentication** – Secure login/register system (planned)
- 📊 **Future Scope** – AI-driven stock suggestions, mutual funds, BSE & global trade support

---

## 🛠 Tech Stack

### ✅ Backend
- **Python 3.10**
- **FastAPI** – Async API framework
- **cachetools** – For TTL cache
- **nse-jugaad-data** – Live stock data from NSE
- **WebSockets** – For real-time communication
- **Uvicorn** – ASGI server

### ✅ Frontend
- **React.js 18**
- **WebSocket API / socket.io-client**
- **Chart.js / D3.js** (optional for portfolio graphs)

### ✅ Node.js Utilities
- **Node.js 18**
- **Express.js 4.18** – Lightweight proxy APIs and utility endpoints

### ✅ Deployment
- **Render** – Backend hosting (due to support for rewrites/redirects)
- **AWS EC2** – For scalable and flexible hosting of backend services

---

---

## ⚠️ Key Challenges & Solutions

### 1. 🧵 Thread-Based API Fetching Bottleneck
- **Issue:** Using one thread per stock caused scalability issues (~8k threads).
- **Fix:** Replaced with `asyncio` in FastAPI for true concurrency.

### 2. 🌐 High Request Volume
- **Issue:** Too many HTTP requests for real-time stock updates.
- **Fix:** Implemented WebSockets + TTL cache to push real-time updates and reduce repeated fetches.

### 3. 🚧 Deployment Limitations
- **Issue:** Vercel didn't support custom rewrites and WebSocket routing.
- **Fix:** Shifted backend to Render and AWS EC2 for full flexibility.

### 4. ❌ 422 Error Handling
- **Issue:** Missing `datetime` dependency in `requirements.txt` caused order timestamps to be `NULL`.
- **Fix:** Added dependency and ensured validation using Pydantic in FastAPI.

---

## 💡 Future Scope

- 🧠 AI-powered suggestion engine (pros/cons before buying a stock)
- 📦 Mutual fund simulation
- 🌍 Support for BSE and global markets
- 🧑‍🤝‍🧑 Social trading (follow & clone portfolios)
- 🏆 Gamification (badges, leaderboards)

---

## 📚 What I Learned

- Fundamentals of **stock trading** and financial data
- Asynchronous programming with **FastAPI + asyncio**
- Real-time systems with **WebSockets**
- Scalable design using **caching and async APIs**
- How to **debug, deploy**, and manage APIs in production-grade environments

---

## 📁 Project Setup

### Backend (FastAPI + WebSocket)
```bash
cd Flask
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
uvicorn combined_app:app --reload

```

### 🌲 Node/Express Services

```bash
cd backend
npm install
node index.js
```

### ⚛️ Frontend (React)

```bash
cd frontend
npm install
npm start
```

```

You can paste this directly into your `README.md` file. Let me know if you want to include environment variable setup or `.env` example too.
```

