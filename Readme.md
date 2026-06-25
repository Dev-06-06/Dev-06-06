# Rahul Dev 👋
**Final Year CSE · Vasavi College of Engineering, Hyderabad**

I build complete products from scratch — from ETL pipelines and ML models to real-time backends, hardware-embedded systems, and React frontends. My work spans fintech intelligence, assistive technology, and real-time systems, with a focus on making data actionable rather than decorative.

Currently seeking SDE roles in product-focused and fintech teams.

---

## Tech Stack

**Frontend**
![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind-06B6D4?style=flat&logo=tailwindcss&logoColor=white)

**Backend**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat&logo=flask&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat&logo=express&logoColor=white)

**Database & Real-Time**
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat&logo=mongodb&logoColor=white)
![Socket.IO](https://img.shields.io/badge/Socket.IO-010101?style=flat&logo=socketdotio&logoColor=white)

**AI / ML**
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat&logo=huggingface&logoColor=black)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini%20API-4285F4?style=flat&logo=google&logoColor=white)

**Data & BI**
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Prophet](https://img.shields.io/badge/Prophet-0077B5?style=flat&logo=meta&logoColor=white)
![PowerBI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)

**Hardware & Embedded**
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat&logo=arduino&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat&logo=cplusplus&logoColor=white)

**Tools & Platforms**
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat&logo=vercel&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?style=flat&logo=render&logoColor=black)
![VSCode](https://img.shields.io/badge/VS%20Code-007ACC?style=flat&logo=visualstudiocode&logoColor=white)

---

## Featured Projects

### 📊 PortSense — AI-Powered Portfolio Analytics
Most Indian retail investors track holdings in Excel or rely on broker apps that only show raw P&L. PortSense goes further — it runs holdings through a FinBERT NLP pipeline for real-time sentiment analysis using fresh GNews articles (with tiered freshness windows per stock), computes portfolio beta and diversification scores, benchmarks returns against Nifty 50 via XIRR, and uses Gemini 2.5 Flash to generate specific rupee-amount rebalancing advice grounded in live data.

Supports NSE stocks, mutual funds (via MFAPI), and fixed deposits — three asset classes in a single unified platform. Features a 13-category market news feed, LTCG/STCG tax classification with inflation-adjusted real returns, a "What If?" comparison against Gold/Silver/Nifty/FD using identical cash flows, and a Stock Intel drawer with sentiment, technicals, and fundamentals — all backed by a 3-tier sector detection system and background analytics prefetching for near-instant page loads.

**Stack:** React · FastAPI · MongoDB Atlas · FinBERT · Gemini 2.5 Flash · yfinance · MFAPI · GNews API  
[🔗 Live Demo](https://bit.ly/portsense) · [API Docs](https://portsense.onrender.com/docs) · [GitHub](https://github.com/Dev-06-06/PortSense)
> 🎯 Demo login: `demo@portsense.in` / `Demo@1234`

---

### 🧤 Silent Voice Glove — Wearable Sign Language Translator
A bidirectional assistive device that closes the communication gap between the deaf/mute community and the hearing world — built entirely from hardware and software components without any third-party translation service.

The glove uses five flex sensors and an MPU6050 IMU on an Arduino Uno to capture per-finger bend angles and wrist orientation. After per-user calibration, gestures are classified against a CSV lookup and served as text through a Flask web interface — offline, no app install required. The reverse flow uses the Web Speech API to transcribe spoken or typed input and map it to sign language video playback. Both directions run in the same local interface, making it genuinely bidirectional without requiring two separate tools.

**Stack:** Arduino C++ · Python · Flask · pyserial · Web Speech API · HTML/CSS/JS  
[▶ Demo Video](https://www.youtube.com/watch?v=nqCvszWmqcc) · [GitHub](https://github.com/Dev-06-06/theme_based_project)

---

### 💰 SmartTax — Dual-Sided Fintech Intelligence Platform
SmartTax is built around one core insight: every UPI transaction is a behavioral signal — most banks ignore it, SmartTax doesn't. It runs two parallel engines on the same underlying data pipeline. The user-facing engine converts transactions into goal-based micro-savings: when a user sets a goal, Prophet forecasts category-level spend, and the ML layer computes inversely-weighted tax percentages per category so that discretionary spending (travel, shopping) absorbs a higher contribution rate than necessities. Every transaction then nudges a small amount toward the goal automatically.

The bank-facing engine uses KMeans segmentation across five behavioral features to cluster customers into Conservative, Moderate, and Aggressive profiles — then surfaces partnership triggers, churn signals, and pre-approved loan candidates through a Power BI layer connected via REST to the Flask backend. The entire data foundation is built on a clean ETL pipeline over a Kaggle banking dataset, generating 50 synthetic users and 7,600+ transactions loaded into MongoDB Atlas.

**Stack:** React · Flask · Python · MongoDB Atlas · Prophet · Scikit-learn · Power BI · Pandas  
[GitHub](https://github.com/Dev-06-06/SmartTax)

---

### 🏏 CricTrack — Real-Time Match Management for Local Cricket
Every cricket scoring app assumes squads are locked before the match, overs never change, and no player appears on both sides. None of that is true in gully or turf cricket. CricTrack is built around these realities — handling late arrivals, mid-game over changes, and a Joker player designation that lets one person bat for one team and bowl for the other, with career stats tracked separately per innings.

The full match lifecycle runs from toss to career stats. The umpire view records every delivery — runs, extras, wickets, bench/replace, undo — syncing instantly across all connected clients via WebSockets. Architecture decisions were made deliberately: embedded player snapshots avoid `populate()` on the hot scoring path, atomic bench-and-replace events eliminate the race condition of recording a delivery mid-swap, and deterministic stat recalculation at match end ensures undos and mid-game changes never produce drift.

**Stack:** React 19 · Node.js · Express · Socket.IO 4 · MongoDB Atlas · TailwindCSS 4 · JWT  
[🔗 Live Demo](https://bit.ly/crictrack) · [GitHub](https://github.com/Dev-06-06/cricket-tracker)

---

## Connect
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rahul-dev-080915304/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/Dev-06-06)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:5343rahuldev@gmail.com)
