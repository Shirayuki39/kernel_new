# Build Android GKI with GitHub Actions  

[![CodeFactor](https://www.codefactor.io/repository/github/hazepynut/gki-builder/badge)](https://www.codefactor.io/repository/github/hazepynut/gki-builder)  

This repository provides an automated workflow to build the **Android Generic Kernel Image (GKI)** using **GitHub Actions**.  
With this setup, you can compile the GKI kernel directly in GitHub’s cloud environment without requiring a powerful local machine.  

## 🚀 Prerequisites  

Before running the workflow, you need to configure some **secrets** in your GitHub repository:  

1. **`GH_TOKEN`** – Your GitHub personal access token, required for uploading build artifacts to the repository.  
   - [How to generate a GitHub Token?](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens)  

2. **`TOKEN`** – Your Telegram bot token, required for sending build notification.
   - [How to create a Telegram bot?](https://www.siteguarding.com/en/how-to-get-telegram-bot-api-token)  

4. **`CHAT_ID`** – The Telegram chat or group ID where the bot will send notifications.  
   - [How to get a Telegram chat ID?](https://www.wikihow.com/Know-Chat-ID-on-Telegram-on-Android)  

### How to Add Secrets to GitHub  
- Follow this guide: [Using secrets in GitHub Actions](https://docs.github.com/en/actions/security-guides/using-secrets-in-github-actions)  

## ⚙️ Configuration  

Before running the workflow, you **must** modify the following files according to your requirements:  

- **`config.sh`** – Contains kernel configuration settings.  
- **`build.sh`** – The main script responsible for compiling the kernel.  

Once configured, you can start building!  

## ✅ Compatibility  

| GKI Version | Support |
|-------------|---------|
| **5.10**    | ✅ Yes  |
| **>5.10**   | ❌ No   |

## 📜 License  

This project is licensed under the **[WTFPL](http://www.wtfpl.net/)**
