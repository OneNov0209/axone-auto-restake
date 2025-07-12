# 🤖 Axone AutoStake Bash Script

This script automates the process of:

- Withdrawing rewards and commission
- Redelegating all available balance (leaving 1 AXONE for gas)
- Sending real-time notifications to Telegram with TX hashes

---

## ⚙️ Requirements

- `axoned` must be installed and synced
- Your validator wallet must be imported
- Telegram Bot Token (get via [BotFather](https://t.me/BotFather))
- Telegram Chat ID (use [@userinfobot](https://t.me/userinfobot))

---

## 🛠 Setup

1. Clone this repo or copy the file:
```bash
chmod +x axone-autostake
