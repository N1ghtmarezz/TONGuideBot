# 🤖 TON Guide Bot — @TONGuideBot

> **Tosha** — your AI guide to the TON blockchain, right inside Telegram.  
> Onboarding, wallets, AI analysis, quiz and more — in 5 minutes.

[![Telegram](https://img.shields.io/badge/Telegram-@TONmassBot-blue?logo=telegram)](https://t.me/TONmassBot)
[![Python](https://img.shields.io/badge/Python-3.10+-green?logo=python)](https://python.org)
[![TON](https://img.shields.io/badge/Blockchain-TON-0088CC?logo=telegram)](https://ton.org)
[![Groq](https://img.shields.io/badge/AI-Groq%20LLaMA%203.3-orange)](https://groq.com)

---
<img width="1536" height="1024" alt="aea2ff1b-e4c7-4cd3-bd95-94dd769dc91d" src="https://github.com/user-attachments/assets/57491f0e-e671-4c2c-a9bd-3cf533f20bed" />
## 🚀 Features

| Feature | Description |
|---------|-------------|
| 🧭 Onboarding | Step-by-step guide from zero to first TON wallet |
| 🤖 AI Assistant | Answers any TON question in natural language (Groq LLaMA 3.3 70B) |
| 🔍 Wallet Analysis | Balance check + AI-generated insight on wallet activity |
| 💱 Price Converter | Live TON → USD / EUR / RUB rates (CoinGecko) |
| 🔎 Transaction Decoder | Explains any TON transaction in plain language |
| 🎯 TON Quiz | 5 questions to test your blockchain knowledge |
| 💡 Fact of the Day | 40+ unique TON ecosystem facts, 3 per day |
| 🚨 Scam Base | Top 13 crypto scam schemes explained by Tosha |
| 🤖 Proactive Notifications | Smart re-engagement scheduler based on user progress |
| 📈 Progress Tracking | Per-user onboarding step tracker |
| 🧠 Long-term Memory | Bot remembers name, topics, visit history |
| 📊 Analytics | Funnel analytics dashboard for admin |

---

## 🏗 Tech Stack

- **Python 3.10+** + **aiogram 3** — Telegram bot with FSM
- **Groq API** (LLaMA 3.3 70B) — AI responses and analysis
- **TONCenter API** — TON blockchain data
- **CoinGecko API** — Live TON price
- **systemd** — Auto-restart and monitoring on VPS
- **JSON** — Progress, memory and analytics storage

---

## ⚡️ Quick Start

### 1. Clone the repository
```bash
git clone https://github.com/N1ghtmarezz/TONGuideBot.git
cd TONGuideBot
```

### 2. Install dependencies
```bash
pip3 install aiogram groq aiohttp python-dotenv
```

### 3. Create `.env` file
```bash
cp env.example .env
# Fill in your keys
```

```env
TELEGRAM_TOKEN=your_telegram_bot_token
GROQ_API_KEY=your_groq_api_key
```

### 4. Run the bot
```bash
python3 bot.py
```

---

## 🗂 Project Structure

```
TONGuideBot/
├── bot.py              # Main bot file
├── .env                # Secrets (not in repo)
├── env.example         # Template for .env
├── .gitignore
├── analytics.json      # User funnel data
├── progress.json       # Onboarding progress per user
├── memory.json         # Long-term user memory
└── notify.json         # Proactive notification state
```

---

## 🔄 Onboarding Flow

```
/start
  └── Fact of the Day + Greeting
        ├── 🛡️ How not to lose money
        │     └── Security explanation → Continue to onboarding
        ├── 🚀 Create TON wallet in 5 minutes
        │     ├── Install Tonkeeper
        │     ├── Create wallet → Share with friend
        │     ├── Get test TON
        │     └── ✅ Check balance → AI analysis → Next steps
        ├── 🔍 Check wallet balance
        ├── 💱 TON price
        ├── 🔎 Decode transaction
        ├── 🎯 TON Quiz → Result → Share with friend
        └── ⚙️ More
              ├── 💡 Fact of the day
              ├── 🚨 Scam base
              └── 📈 My progress
```

---

## 📊 Metrics (since launch)

- 👥 **31** unique users
- 🚀 **101** bot starts
- 💬 **187** AI questions asked
- ✅ **24** users created a wallet

---

## 🎯 Hackathon

Built for **TON AI Agent Hackathon 2026**.  
Track: User-Facing AI Agents.

**Ecosystem value:**
- Lowers the entry barrier for newcomers
- Teaches through dialogue, not documentation
- Prepares users for Proof of Onboarding NFT
- Every new Telegram user is a potential TON user. Tosha meets them first.

---

## 🗺 Roadmap

- 🏆 **TON Achievement System** — points, NFT tiers (Common / Rare / Epic), referral system
- 🎨 **Mini App** — user profile, leaderboard, achievement showcase
- 🎖️ **Proof of Onboarding NFT** — auto-mint after completing full onboarding

---

## 👤 Author

**Mr. N1ghtmare** — [@N1ghtmarezz](https://github.com/N1ghtmarezz)

---

## 📄 License

MIT
