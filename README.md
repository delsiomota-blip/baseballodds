# ⚾ MLB Matchup Analytics v5.1

**Live MLB Data • Edge Detection • Smart Parlay Builder**

A clean, stable Streamlit application for MLB betting analysis with real-time data from MLB Stats API and pybaseball (Statcast).

---

## ✨ Features

### 📅 Today's Games
- Real-time MLB schedule from official API
- Starting pitchers
- Clean table view

### 🔎 Matchup Analysis
- Player stats from Statcast (last 7 days)
- **Edge Score** = (xwOBA × 0.5) + (ParkFactor × 0.3) − (K% × 0.2)
- FanGraphs-style metrics: wRC+, FIP, WAR
- Value bet detection

### 🎰 Parlay Builder
- Automatically generates **3 optimized parlays**
- 2-leg (Super Seguro), 3-leg (Seguro), 3-leg (Value)
- No repeated players across parlays
- Estimated combined odds

### ⚙️ Settings
- Adjustable minimum Edge threshold
- Toggle for real vs fallback data

---

## 🚀 Quick Start

### Prerequisites
- Python 3.10+
- pip
- Internet connection (for real data)

### Local Installation

```bash
cd /home/workdir/artifacts
pip install -r requirements.txt
streamlit run app.py
```

The app will open automatically at **http://localhost:8501**

### Access from Another Device
1. Find your computer's local IP (`ipconfig` on Windows / `ifconfig` on Mac/Linux)
2. Open `http://YOUR-IP:8501` on your phone or tablet

### Deploy to Streamlit Cloud (Free)
1. Push this repo to GitHub
2. Go to [share.streamlit.io](https://share.streamlit.io)
3. Connect your repo and deploy
4. Your app will be live at `https://your-app-name.streamlit.app`

---

## 🛠 Tech Stack

| Component       | Technology                     |
|-----------------|--------------------------------|
| Framework       | Streamlit 1.32+                |
| Data            | pandas, numpy                  |
| Real Data       | MLB Stats API + pybaseball     |
| Caching         | Streamlit @st.cache_data       |

---

## 📄 License

MIT License

---

**Version 5.1 — Improved with FanGraphs metrics + Full 3-Parlay Builder**