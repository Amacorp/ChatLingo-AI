# ChatLingo AI — Translator for WhatsApp & Slack

> **Type in your language, send in theirs.**
>
> A Chrome extension that adds AI-powered, real-time translation directly into **WhatsApp Web** and **Slack Web**. No copy-pasting, no app-switching — just type, click **T-Send**, and your message is translated and sent in one smooth motion.

![Platforms](https://img.shields.io/badge/platforms-WhatsApp%20Web%20%7C%20Slack%20Web-blue)
![Languages](https://img.shields.io/badge/languages-11-green)
![Providers](https://img.shields.io/badge/AI%20providers-Cerebras%20%7C%20Gemini%20%7C%20OpenAI-orange)
![License](https://img.shields.io/badge/license-MIT-purple)
![Price](https://img.shields.io/badge/price-100%25%20FREE-success)

**Templates, setups, and streaming happen entirely on your machine. No proxy servers, 100% private.**

---

### 👨‍💻 Author
**Mehdi Ghahramanian**
* [LinkedIn](https://www.linkedin.com/in/m-gakhramanian/)
* [GitHub](https://github.com/Amacorp/ChatLingo-AI)

---

## ✨ Features

* **Outgoing Translation:** Type in your native language, click **T-Send**, and watch it stream, translate, and automatically send.
* **Translate-Only Mode:** Press `Ctrl+Shift+T` (`⌘+Shift+T` on Mac) to preview and edit the translation before hitting send.
* **Incoming Translation:** Hover over any received message and click the **🌐** icon to view its translation right below the text.
* **BYO Key:** Bring your own API key (Cerebras, Gemini, or OpenAI). Zero telemetry, zero middle-man logging.

---

## 🌍 Supported Languages

Supports cross-translation between any of these **11 languages**:

Persian (`fa`), English (`en`), German (`de`), Russian (`ru`), Spanish (`es`), Chinese (`zh`), Japanese (`ja`), French (`fr`), Portuguese (`pt`), Italian (`it`), Turkish (`tr`).

---

## 📦 Installation & Setup

1. Clone or download this repository.
2. Open Chrome and head to `chrome://extensions/`.
3. Toggle on **Developer mode** (top right).
4. Click **Load unpacked** and select the extension folder containing `manifest.json`.
5. Click the extension toolbar icon to open **Settings**.
6. Input your API key, select your language mapping, and hit **Save**.

---

### Framework Challenges Handled:
* **WhatsApp Web:** Overcomes React's controlled `contenteditable` state by programmatically triggering a synthetic `ClipboardEvent('paste')` coupled with async DOM polling to prevent input desync.
* **Slack Web:** Interacts cleanly with the underlying Quill editor infrastructure using native DOM command inserts to allow live token streaming.

---

## 🐛 Troubleshooting Quick-Fix

* **No T-Send Button?** Ensure you have typed at least one character. WhatsApp hides send components on empty inputs.
* **Paste Failures (WhatsApp)?** Clear the box manually (`Ctrl+A` -> `Backspace`), click into the input field to re-focus, and try again.
* **API Errors:** Check your console (F12). 
  * `401`: Key invalid. 
  * `429`: Rate limited.

---

## 📝 License

Distributed under the **MIT License**. Feel free to fork, modify, and distribute.
