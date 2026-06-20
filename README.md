# ChatLingo AI — Translator for WhatsApp, Telegram & Slack

> **Type in your language, send in theirs.**
>
> A Chrome extension that adds AI-powered, real-time translation directly into **WhatsApp Web**, **Telegram Web**, and **Slack Web**. No copy-pasting, no app-switching — just type, click **T-Send**, and your message is translated and sent in one smooth motion.

![Platforms](https://img.shields.io/badge/platforms-WhatsApp%20%7C%20Telegram%20%7C%20Slack-blue)
![Languages](https://img.shields.io/badge/languages-11-green)
![Providers](https://img.shields.io/badge/AI%20providers-Cerebras%20%7C%20Gemini%20%7C%20OpenAI-orange)
![License](https://img.shields.io/badge/license-MIT-purple)
![Price](https://img.shields.io/badge/price-100%25%20FREE-success)
![Version](https://img.shields.io/badge/version-4.1.0-blue)

**🆓 100% Free forever.** No subscriptions, no ads, no data collection. Open-source.

---

### 👨‍💻 Author

**Mehdi Ghahramanian**
- 💼 [LinkedIn](https://www.linkedin.com/in/m-gakhramanian/)
- 🐙 [GitHub](https://github.com/Amacorp/ChatLingo-AI)

*Powered with ❤️ by Mehdi Ghahramanian*

---

### 🤝 Support & Community

- 🐛 **Found a bug?** [Open an issue](https://github.com/Amacorp/ChatLingo-AI/issues)
- 💡 **Have a feature idea?** [Start a discussion](https://github.com/Amacorp/ChatLingo-AI/discussions)
- 🛠️ **Want to contribute?** Pull requests are welcome!
- ⭐ **Like the extension?** Star the repo — it helps others discover it.

---

## ✨ What it does

ChatLingo AI integrates a translation layer directly into the chat apps you already use. Once installed, you get three powerful capabilities:

### 1. Outgoing translation — *Type in your language, send in theirs*

Type your message in **your** language (e.g. Persian), then click the blue **T-Send** button that appears next to WhatsApp's, Telegram's, or Slack's send button. The extension:

1. Reads what you typed
2. Sends it to your chosen AI provider (Cerebras / Gemini / OpenAI)
3. Streams the translation back into the input box
4. Clicks send for you

The result: your teammate receives a clean, professional message in their language.

### 2. Translate-only mode — *Review before sending*

Prefer to review the translation before it goes out? Press <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>T</kbd> (or <kbd>⌘</kbd>+<kbd>Shift</kbd>+<kbd>T</kbd> on macOS). The translation fills the input box but **isn't sent** — you can edit it, then press <kbd>Enter</kbd> when ready.

### 3. Incoming translation — *Understand messages in any language*

Every incoming message gets a small **🌐** button in its corner. Click it, and a translation panel appears right below the message — translated into your "I type in" language. Perfect for understanding teammates who write in languages you don't read.

---

## 🌍 Supported languages

11 languages, covering the most-used scripts and regions:

| Code | Language | Native name | Script |
|------|----------|-------------|--------|
| `fa` | Persian (Farsi) | فارسی | Arabic (RTL) |
| `en` | English | English | Latin |
| `de` | German | Deutsch | Latin |
| `ru` | Russian | Русский | Cyrillic |
| `es` | Spanish | Español | Latin |
| `zh` | Chinese | 中文 | Han |
| `ja` | Japanese | 日本語 | Kana / Kanji |
| `fr` | French | Français | Latin |
| `pt` | Portuguese | Português | Latin |
| `it` | Italian | Italiano | Latin |
| `tr` | Turkish | Türkçe | Latin |

**Any pair works.** Persian → English, French → Russian, Chinese → Japanese, Spanish → German, Turkish → French — the AI handles every combination. You're never locked into "translate to English."

---

## 🤖 AI providers

ChatLingo AI works with three leading AI providers. Bring your own API key — the extension never proxies your data through any third-party server.

| Provider | Recommended model | Get an API key |
|----------|-------------------|----------------|
| **Cerebras AI** | `zai-glm-4.7` | [cloud.cerebras.ai](https://cloud.cerebras.ai/) |
| **Google Gemini** | `gemini-2.0-flash-exp` | [aistudio.google.com/apikey](https://aistudio.google.com/apikey) |
| **OpenAI** | `gpt-4o-mini` | [platform.openai.com/api-keys](https://platform.openai.com/api-keys) |

All three providers stream tokens back in real time, so you see the translation appear word-by-word in your input box. On Slack, the streaming is visible as it happens; on WhatsApp and Telegram, the final translation is applied in one shot (to avoid React state desync issues).

---

## 📦 Installation

ChatLingo AI is a **Manifest V3** Chrome extension. Load it manually:

1. **Download or clone** this repository to your computer.
2. Open Chrome and navigate to `chrome://extensions/`.
3. Toggle on **Developer mode** (top-right corner).
4. Click **Load unpacked**.
5. Select the folder containing `manifest.json`.
6. The ChatLingo AI icon appears in your toolbar. Click it to open Settings.

> **Edge / Brave / Opera / Vivaldi** — same instructions. These browsers are Chromium-based and support MV3 extensions.

---

## ⚙️ First-time setup

1. **Click the ChatLingo AI toolbar icon** → Settings page opens.
2. **Pick a provider** (Cerebras, Gemini, or OpenAI).
3. **Paste your API key** for that provider.
4. **Choose a model** (the default is fine for most users).
5. **Set your languages**:
   - **"I type in"** — the language you'll write messages in
   - **"Translate outgoing to"** — the language your messages get translated to
6. **(Optional)** Toggle "Show 🌐 button on incoming messages" on or off.
7. **Click Save**.

You can use the built-in **Test translation** panel on the settings page to verify your API key works before heading to your chat app.

---

## 🚀 Usage

### On WhatsApp Web (`web.whatsapp.com`)

1. Open a chat and click into the message input box.
2. Type your message in your "I type in" language.
3. **Click the blue T-Send button** (it appears to the left of WhatsApp's send button).
4. Watch the "Translating…" indicator, then your message is sent in the target language.

### On Telegram Web (`web.telegram.org`)

1. Open a chat and click into the message input box.
2. Type your message in your "I type in" language.
3. **Click the blue T-Send button** (it appears to the left of Telegram's send button).
4. Watch the "Translating…" indicator, then your message is sent in the target language.

> **Note:** Telegram Web has three variants (`/a/`, `/k/`, `/z/`). All are supported. The extension uses smart DOM discovery to find the send button regardless of which variant you're on.

### On Slack Web (`app.slack.com`)

1. Open a channel or DM and click into the message input.
2. Type your message in your "I type in" language.
3. **Click the blue T-Send button** next to Slack's send button — translates and sends.
4. **Or press <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>T</kbd>** to translate only (review before sending).

### Translating incoming messages

1. Make sure "Show 🌐 button on incoming messages" is enabled in Settings.
2. Hover any incoming message — you'll see a small **🌐** button.
3. Click it — a translation panel appears below the message, in your "I type in" language.
4. Click the **×** on the panel to dismiss it.

---

## ⌨️ Keyboard shortcuts

| Shortcut | Action |
|----------|--------|
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>T</kbd> (Windows/Linux) | Translate current input (no auto-send) |
| <kbd>⌘</kbd>+<kbd>Shift</kbd>+<kbd>T</kbd> (macOS) | Translate current input (no auto-send) |

Click inside the message box first, then press the shortcut. Works on all three platforms (WhatsApp, Telegram, Slack).

---

## 🔒 Privacy & data flow

ChatLingo AI is built privacy-first:

- **Your API key** is stored in `chrome.storage.local` — on your machine, never on any server.
- **Your messages** are sent directly from your browser to your chosen AI provider's API. No middleware, no proxy, no logging.
- **No analytics, no telemetry, no tracking.** The extension doesn't phone home.
- **No account required.** You bring your own API key; that's the only identity involved.

The extension requests these permissions:

| Permission | Why |
|------------|-----|
| `storage` | Save your API key, language preferences, and settings locally |
| `activeTab` | Detect which chat app you're on (WhatsApp / Telegram / Slack) |
| Host: `web.whatsapp.com` | Inject the T-Send button and translate incoming messages |
| Host: `web.telegram.org` | Same — inject UI into Telegram Web |
| Host: `app.slack.com` | Same — inject UI into Slack |
| Host: provider APIs | Send translation requests to Cerebras / Gemini / OpenAI |

That's it. No `tabs`, no `history`, no `cookies`, no `<all_urls>`.

---

## 🎨 The T-Send button

The T-Send button is the heart of ChatLingo AI. It appears next to the native send button on all three supported platforms:

- **WhatsApp & Telegram** — a 40×40 round button with a gradient blue background, dark blue border, and the white ChatLingo language icon centered. The border and gradient ensure maximum visibility against any chat background.
- **Slack** — a compact pill button (32px height) with the same gradient blue + dark blue border, the language icon, and a "T-Send" label.

**Button states:**
- **Normal** — gradient blue (`#3b82f6` → `#1d4ed8`) with dark blue border (`#1e3a8a`)
- **Hover** — darker gradient (`#2563eb` → `#1e40af`) with stronger shadow
- **Active (pressed)** — scaled to 92–96%
- **Busy (translating)** — gray gradient, pointer disabled

The button uses CSS `!important` on critical properties to override any inherited styles from the host chat app, ensuring it always looks consistent.

---

## 🏗️ How it works (technical overview)

ChatLingo AI is a single content script (`content.js`) that detects the host platform on load and dispatches to a platform-specific adapter. All translation logic, the streaming port to the background service worker, the language catalog, and the UI helpers are shared.

```
┌──────────────────────────────────────────────────────────────────┐
│  content.js (content script, runs on WhatsApp, Telegram & Slack)  │
│                                                                  │
│  ┌────────────┐  ┌──────────────┐  ┌──────────┐  ┌────────────┐  │
│  │ SlackAdapter│  │WhatsAppAdapter│  │TelegramAd│  │Shared logic│  │
│  │ • selectors │  │ • selectors   │  │• smart   │  │• translate │  │
│  │ • send msg  │  │ • send msg    │  │ btn find │  │• streaming │  │
│  │ • inject UI │  │ • inject UI   │  │• inject  │  │• UI factory│  │
│  └────────────┘  └──────────────┘  └──────────┘  └─────┬──────┘  │
│                                                        │         │
└────────────────────────────────────────────────────────┼─────────┘
                                                         │
                                                chrome.runtime.connect
                                                         │
┌────────────────────────────────────────────────────────▼─────────┐
│  background.js (service worker)                                   │
│                                                                   │
│  • Receives { text, source, target } via long-lived port          │
│  • Calls provider API (Cerebras / Gemini / OpenAI)                │
│  • Streams partial translations back via { type:'partial' }       │
│  • Sends final translation via { type:'done' }                    │
└───────────────────────────────────────────────────────────────────┘
```

### Platform-specific handling

**Slack Web (Quill-based contenteditable):** Slack uses Quill, which respects `document.execCommand('insertText')`. Streaming partials appear live in the input as the LLM generates them.

**WhatsApp & Telegram Web (React-based contenteditable):** Both apps use React-controlled `contenteditable` divs where React is the single source of truth — direct DOM manipulation gets reverted. The most reliable approach is:

1. Focus the input and select all its content via the Range API
2. Dispatch a single synthetic `ClipboardEvent('paste')` with the translated text in a `DataTransfer` object
3. Poll the DOM asynchronously (up to 2 seconds) for React to process the paste
4. Only then click the send button

This avoids the duplication bugs that arise from fighting React's state management.

### Telegram Web: smart send-button discovery

Telegram Web has three variants (`/a/`, `/k/`, `/z/`) with frequently-changing DOM. Instead of relying on fixed selectors, the Telegram adapter uses a **two-phase discovery** approach:

1. **Phase 1:** Try common send-button selectors (`button[aria-label*="Send"]`, `button[class*="send"]`, etc.)
2. **Phase 2:** Find the message input, walk up to its composer container, find ALL buttons inside it, and pick the **rightmost** one (the send button is almost always the rightmost button in the composer)

This spatial heuristic works regardless of what class names or aria-labels Telegram uses.

---

## 🐛 Troubleshooting

### "Translation did not apply" toast on WhatsApp or Telegram

This means the paste approach failed. Try:

1. **Clear the input box** (Ctrl+A → Delete).
2. **Click into the input box** to ensure it has focus.
3. **Click T-Send again.**

If it keeps failing, open DevTools Console (F12) and look for `[PT]` logs — they'll show exactly which step failed.

### The T-Send button doesn't appear

- Make sure you've **typed at least one character** — WhatsApp and Telegram hide the send button (and show a mic/attach icon) when the input is empty.
- **Refresh the page** — sometimes the page's initial render happens before the extension loads.
- Open DevTools Console and check for `[ChatLingo AI]` logs — if there's no "loaded on platform" line, the extension didn't load.

### T-Send button appears in the wrong position on Telegram

Telegram's DOM can vary. The adapter uses smart discovery, but if the button lands in an odd spot, **refresh the page** — the adapter re-evaluates the layout on every MutationObserver tick.

### Same-language warning

If you see "⚠️ Source and target are both X", open Settings and pick a different "Translate outgoing to" language.

### API errors (401, 403, 429, 500)

| Status | Meaning | Fix |
|--------|---------|-----|
| 401 | Invalid API key | Re-paste your key in Settings |
| 403 | Key doesn't have access to the model | Try a different model |
| 404 | Model not found | Check the model name in Settings |
| 429 | Rate-limited | Wait a few seconds and retry |
| 5xx | Provider server error | Try again shortly |

---

## 📁 File structure

```
chatlingo-ai/
├── manifest.json       # MV3 manifest — name, permissions, scripts, icons
├── content.js          # Content script (runs on WhatsApp, Telegram & Slack)
├── background.js       # Service worker (handles API calls & streaming)
├── options.html        # Settings page UI
├── options.js          # Settings page logic
├── icons/              # Extension icons (gradient blue with dark border)
│   ├── icon16.png      # 16×16  — toolbar (small)
│   ├── icon32.png      # 32×32  — toolbar (large), favicon
│   ├── icon48.png      # 48×48  — extensions page
│   ├── icon128.png     # 128×128 — store listing, settings header
│   ├── favicon.png     # 32×32  — settings page favicon
│   └── icon.svg        # Source SVG
└── README.md           # This file
```

---

## 🔄 Version history

| Version | Highlights |
|---------|------------|
| **4.1.0** | T-Send button redesigned with gradient blue + dark blue border for better visibility. Icons regenerated to match (gradient + border + 3D highlight). README updated for GitHub. |
| **4.0.0** | **Added Telegram Web support.** Now supports all three major chat platforms: WhatsApp, Telegram, and Slack. Telegram adapter uses smart send-button discovery (two-phase: direct selectors + spatial heuristic). Renamed WhatsApp-specific functions to be React-generic. |
| **3.1.0** | New extension icons (blue, Clarity language-line). Unified blue T-Send button on WhatsApp & Slack. Slack adapter upgraded to single-global-button approach. Favicon added to settings page. |
| **3.0.0** | Renamed to ChatLingo AI. Redesigned settings UI. README. Reduced to 11 core languages. Removed unreliable language detection. Robust WhatsApp paste approach with async polling. Single global T-Send button (no duplicates). |
| 2.x | Multi-strategy text replacement, retry mechanisms, single-button injection, anti-duplicate cleanup, paste-event approach. |
| 1.x | Initial release. Slack support. Persian → English focus. |

---

## 📝 License

MIT — use it, fork it, ship it.

---

## 💡 Tips

- **Swap languages instantly** with the ⇄ button in Settings — useful when you're bilingual and switch between writing in either language.
- **The "Test translation" panel** in Settings is great for verifying your API key works without leaving the page.
- **The diagnostic panel** at the bottom of Settings shows exactly what's stored in `chrome.storage.local` — useful if something seems misconfigured.
- **Click the toolbar icon** any time to jump back to Settings.
- **Works on all three platforms simultaneously** — set your languages once, and use ChatLingo AI on WhatsApp, Telegram, and Slack without reconfiguring.

---

## 🌟 Why ChatLingo AI?

- ✅ **Three platforms, one extension** — WhatsApp, Telegram, and Slack
- ✅ **11 languages, any pair** — not just "translate to English"
- ✅ **Three AI providers** — Cerebras, Gemini, or OpenAI (bring your own key)
- ✅ **Streaming translations** — see the text appear in real time
- ✅ **Incoming translation** — understand messages in any language
- ✅ **100% free, no ads, no tracking** — privacy-first
- ✅ **Open-source** — MIT licensed, contributions welcome
- ✅ **Production-ready** — polished UI, robust error handling, comprehensive docs

---

**Made with care for people who work across languages.** 🌐
