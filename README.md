Here's the English version while preserving all the markdown formatting:

# 🤖 Axone AutoStake

Automated shell script to withdraw rewards and instantly redelegate (re-stake) to your Axone validator. Features real-time Telegram notifications.

## ✨ Features

- Automatic reward + commission withdrawal (`withdraw-rewards --commission`)
- Instant re-delegation from remaining balance (keeps 1 AXONE for fees)
- Telegram notifications for:
  - Withdrawal TX Hash
  - Stake TX Hash
  - Re-stake amount
  - Status and timestamp

## ⚠️ Requirements

- Active `axoned` validator node
- Validator wallet imported to node
- `jq`, `bc`, and `curl` installed
- Telegram Bot token from [BotFather](https://t.me/BotFather)
- Chat ID from [@userinfobot](https://t.me/userinfobot)
---
## 🛠️ Setup

1. Clone this repository:
```bash
git clone https://github.com/OneNov0209/axone-auto-restake.git
cd axone-auto-restake
chmod +x axone-autostake
```

2. Edit configuration:
```bash
nano axone-autostake
```
Update these values:
```bash
VALOPER="axonevaloper1xxxxxxxxxxxxxxxxxxxxx"
WALLET="wallet"
BOT_TOKEN="your_bot_token_here"
CHAT_ID="your_chat_id_here"
```

## 🚀 Usage

### Manual run:
```bash
./axone-autostake
```

### Automated (daily at 7:00 UTC via cron):
```bash
crontab -e
```
Add this line:
```bash
0 7 * * * /path/to/axone-auto-restake/axone-autostake >> /var/log/axone-autostake.log 2>&1
```

## 📨 Telegram Notification Example

```
✅ [Axone AutoStake]

✅ Withdrawal successful
🔗 https://explorer.onenov.xyz/axone-mainnet/tx/XXXX...

✅ Re-Stake completed
💰 Amount: 13.9523 AXONE
🔗 https://explorer.onenov.xyz/axone-mainnet/tx/YYYY...

⏰ Date: 2025-07-12 07:00 UTC
✅ Status: Success
```

## 👤 Author

Created with ❤️ by [OneNov](https://onenov.xyz)

---

## 📜 License

Open-source - fork and use freely
```

Key changes made:
1. Translated all Indonesian text to English
2. Maintained all original markdown formatting (headers, code blocks, lists)
3. Preserved all links and technical terms
4. Kept the same emoji usage
5. Maintained identical structure and section ordering
6. Preserved all code blocks and bash commands exactly as-is
7. Kept the same line breaks and spacing

The document is now fully in English while being functionally identical to the original in terms of formatting and structure.
