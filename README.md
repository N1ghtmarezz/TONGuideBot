# 🤖 TON Guide Bot — @TONGuideBot

> **Тоша** — твой AI-гид по TON блокчейну прямо в Telegram.  
> Онбординг, кошельки, AI-анализ, квиз и многое другое — за 5 минут.

[![Telegram](https://img.shields.io/badge/Telegram-@TONmassBot-blue?logo=telegram)](https://t.me/TONmassBot)
[![Python](https://img.shields.io/badge/Python-3.10+-green?logo=python)](https://python.org)
[![TON](https://img.shields.io/badge/Blockchain-TON-0088CC?logo=telegram)](https://ton.org)
[![Groq](https://img.shields.io/badge/AI-Groq%20LLaMA%203.3-orange)](https://groq.com)

---
<img width="1536" height="1024" alt="aea2ff1b-e4c7-4cd3-bd95-94dd769dc91d" src="https://github.com/user-attachments/assets/57491f0e-e671-4c2c-a9bd-3cf533f20bed" />

## 🚀 Что умеет бот

| Фича | Описание |
|------|----------|
| 🧭 Онбординг | Пошаговый гайд от нуля до первого TON кошелька |
| 🤖 AI-ассистент | Отвечает на любые вопросы про TON (Groq LLaMA 3.3 70B) |
| 🔍 Анализ кошелька | Проверка баланса + AI-инсайт по активности |
| 💱 Конвертер | Живой курс TON → USD / EUR / RUB (CoinGecko) |
| 🔎 Расшифровка транзакций | Объясняет любую TON транзакцию простым языком |
| 🎯 TON-квиз | 5 вопросов для проверки знаний о блокчейне |
| 💡 Факт дня | 40+ уникальных фактов о TON экосистеме, 3 в день |
| 📈 Прогресс | Трекинг шагов онбординга каждого пользователя |
| 🧠 Долгосрочная память | Бот помнит имя, темы вопросов, историю визитов |
| 📊 Аналитика | Воронка пользователей для администратора |

---

## 🏗 Стек технологий

- **Python 3.10+** + **aiogram 3** — Telegram бот с FSM
- **Groq API** (LLaMA 3.3 70B) — AI-ответы и анализ
- **TONCenter API** — данные блокчейна TON
- **CoinGecko API** — живой курс TON
- **systemd** — автозапуск и мониторинг на VPS
- **JSON** — хранение прогресса, памяти и аналитики

---

## ⚡️ Быстрый старт

### 1. Клонируй репозиторий
```bash
git clone https://github.com/N1ghtmarezz/TONGuideBot.git
cd TONGuideBot
```

### 2. Установи зависимости
```bash
pip3 install aiogram groq aiohttp python-dotenv
```

### 3. Создай `.env` файл
```bash
cp .env.example .env
# Заполни своими ключами
```

```env
TELEGRAM_TOKEN=your_telegram_bot_token
GROQ_API_KEY=your_groq_api_key
```

### 4. Запусти бота
```bash
python3 bot.py
```

---

## 🗂 Структура проекта

```
TONGuideBot/
├── bot.py              # Основной файл бота
├── .env                # Секреты (не в репо)
├── .env.example        # Шаблон для .env
├── .gitignore
├── analytics.json      # Воронка пользователей
├── progress.json       # Прогресс онбординга
└── memory.json         # Долгосрочная память
```

---

## 🔄 Флоу онбординга

```
/start
  └── Факт дня + Приветствие
        ├── 🛡️ Как не потерять деньги
        │     └── Объяснение безопасности → Продолжить
        └── 🚀 Создать TON кошелёк за 5 минут
              ├── Установить Tonkeeper
              ├── Создать кошелёк
              ├── Получить тестовые TON
              └── ✅ Проверить баланс → AI-анализ
```

---

## 📊 Метрики (с момента запуска)

- 👥 **31** уникальных пользователей
- 🚀 **98** стартов бота  
- 💬 **185** AI-вопросов задано
- ✅ **24** пользователя создали кошелёк

---

## 🎯 Хакатон

Проект создан в рамках **TON AI Agent Hackathon 2026**.  
Трек: AI Agent для онбординга новых пользователей в TON экосистему.

**Ценность для экосистемы:**
- Снижает барьер входа для новичков
- Обучает через диалог, а не документацию  
- Готовит пользователей к Proof of Onboarding NFT

---

## 👤 Автор

**Mr. N1ghtmare** — [@N1ghtmarezz](https://github.com/N1ghtmarezz)

---

## 📄 Лицензия

MIT
