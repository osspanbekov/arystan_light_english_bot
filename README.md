# Telegram Automation Assistant for English School

Production-ready Telegram assistant built to automate **client onboarding, lesson booking, and basic support workflows** for an English language school.

The bot replaces manual messaging with structured conversation flows, enabling faster responses and 24/7 availability without increasing staff.

---

## Overview

This project automates repetitive client interactions such as:
- onboarding new students,
- collecting lesson preferences,
- booking lessons,
- handling basic inquiries.

Designed as a long-running production service, not a demo or chatbot prototype.

---

## Key Features

- Automated onboarding and booking flows  
- Input validation and structured conversation logic  
- Persistent data storage for client information  
- Deployed on a Linux VPS with `systemd` for reliability  
- 24/7 availability with automatic restarts

---

## Business Impact

- Reduced response and scheduling time from **hours to minutes**
- Enabled **24/7 client interaction** without additional headcount
- Lowered administrative workload through automation
- Improved consistency of client communication

---

## Architecture

Telegram User  
→ Telegram Bot API  
→ Python Application  
→ Conversation Logic & Validation  
→ Data Storage

---

## Tech Stack

- **Language:** Python  
- **API:** Telegram Bot API  
- **Deployment:** Linux VPS  
- **Process Management:** systemd  

---

## Setup

```bash
git clone https://github.com/osspanbekov/arystan_light_english_bot.git
cd arystan_light_english_bot
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

### Create a .env file:
BOT_TOKEN=your_bot_token_here

### Run the bot:
```bash
python arys_bot.py
```

## Production Notes
### The service is designed to run continuously and is managed via systemd, ensuring stability and automatic recovery.