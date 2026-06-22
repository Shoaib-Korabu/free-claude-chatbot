<div align="center">

# Free Claude Chatbot

**A completely free Claude AI chatbot that runs in your browser. No API key needed. Powered by [Puter.js](https://puter.com).**

[🌐 Live Demo](https://YOUR-GITHUB-USERNAME.github.io/free-claude-chatbot/) · [GitHub](https://github.com/YOUR-GITHUB-USERNAME/free-claude-chatbot)

</div>

---

## 📋 Table of Contents

- [About](#-about)
- [Features](#-features)
- [Live Demo](#-live-demo)
- [Run It Locally](#-run-it-locally)
- [Troubleshooting](#-troubleshooting)
- [License](#-license)

---

## 📖 About

This is a single-file web chatbot that lets you talk to Claude AI models for **free**, directly in your browser.

It works by using **[Puter.js](https://puter.com)** — a free service that handles the Claude API calls through your own Puter account. You don't need an Anthropic API key. You don't need a paid subscription. You just need a free Puter account.

> 🧠 **Single-Use Memory:** Please note that this chatbot operates as a "use-and-throw" interface. It does not retain any memory of previous messages. Whatever context you need the AI to understand must be provided entirely within a single message.

> ⚠️ **Puter's free tier has usage limits** that are not publicly documented. For casual personal use it works well, but heavy or continuous use may hit those limits.

---

## ✨ Features

- 🆓 **Completely free** — no API key, no subscriptions, no hidden costs
- 🤖 **Multiple Claude models** — switch between Sonnet, Opus, Haiku and more from a dropdown
- 🗑️ **Single-Use Interactions** — no conversational memory, perfect for quick, standalone tasks
- ⚡ **Streaming support** — see responses appear word-by-word as they're generated
- 🌙 **Dark theme** — easy on the eyes
- 📄 **One file** — the entire chatbot is a single `index.html` file, nothing else needed

---

## 🌐 Live Demo

👉 **[Open the chatbot](https://YOUR-GITHUB-USERNAME.github.io/free-claude-chatbot/)**

When you open it for the first time:

1. Click **"Sign in to Puter"** — a popup will appear
2. Create a free Puter account, or sign in if you already have one
3. Once the dot next to "Signed in" turns green, you're ready
4. Type your message and press **Enter** (or **Shift+Enter** for a new line)

---

## 💻 Run It Locally

You can also download and run the chatbot on your own computer.

> ⚠️ **Important:** You cannot just double-click the file. Opening it as `file://` is blocked by Puter.js for security reasons. It must be served through a local web server. Three easy ways to do that:

### Option 1 — Python (recommended, no extra install needed on Mac/Linux)

1. Download `index.html` from this repo
2. Open a terminal (or Command Prompt on Windows) in the same folder
3. Run:
   - **Mac / Linux:** `python3 -m http.server 8000`
   - **Windows:** `python -m http.server 8000` or `py -m http.server 8000`
4. Open your browser and go to: `http://localhost:8000`

### Option 2 — Node.js

If you have Node.js installed, run this in the same folder:

```bash
npx serve .
```

Then open the address it prints (usually `http://localhost:3000`).

### Option 3 — VS Code Live Server (no terminal needed)

1. Install the **[Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)** extension in VS Code
2. Open the folder containing `index.html` in VS Code
3. Right-click `index.html` → **"Open with Live Server"**

> ✅ The key thing: your browser's address bar must start with `http://localhost:...` — never `file://`

---

## 🔧 Troubleshooting

### ❌ "Puter.js Error: Unsupported Protocol"

You opened the file by double-clicking it. Puter.js does not allow `file://` for security reasons. Follow the [Run It Locally](#-run-it-locally) steps above — or just use the [Live Demo](#-live-demo) link instead.

### ❌ Sign-in popup doesn't appear

Your browser blocked the popup. Look for a small blocked-popup icon in the address bar and click **Allow**.

### ❌ The page loads but nothing happens after sign-in

Check the **Debug log** section at the bottom of the page — it timestamps every step and will show what went wrong.

### ❌ A model isn't working

Some model names may change or become unavailable over time. Try switching to a different model using the dropdown menu at the top.

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.
