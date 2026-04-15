# VisionBridge — AI Eyes for Everyone

> Real-time AI-powered vision assistance for the visually impaired. Describe surroundings, read text, navigate obstacles, and trigger emergency mode — all through your phone's camera and voice.

## ✨ Features

| Mode | What it does |
|------|-------------|
| **Describe** | AI describes the scene ahead — objects, distances, hazards |
| **Read** | Reads all visible text aloud (signs, labels, menus, medicine) |
| **Navigate** | Live turn-by-turn obstacle guidance while walking |
| **Emergency** | SOS mode — scans for nearest exit and safe path |

### Additional Capabilities
- 🎤 **Voice Commands** — say "describe", "read", "navigate", "stop", or "emergency"
- 🔇 **Stop Speech** — instantly silence AI voice output
- ✕ **Cancel Analysis** — abort any in-progress scan
- ⌨️ **Keyboard Shortcuts** — `D` `R` `N` `Space` `M` `S` `Esc`
- 📱 **Mobile-First** — designed for one-handed phone use
- ♿ **Fully Accessible** — ARIA labels, screen reader support, high contrast UI

## 🚀 Getting Started

### 1. Deploy (HTTPS Required for Camera)

Camera access requires HTTPS. Choose one:

| Method | Steps |
|--------|-------|
| **GitHub Pages** | Push to repo → Settings → Pages → Deploy from `main` |
| **Netlify Drop** | Rename to `index.html` → drag folder to [app.netlify.com/drop](https://app.netlify.com/drop) |
| **Local Dev** | Use VS Code Live Server or `python -m http.server` |

### 2. Get a Free API Key

**Google Gemini (recommended — completely free):**
1. Go to [aistudio.google.com/apikey](https://aistudio.google.com/apikey)
2. Sign in with Google → Create API Key
3. Paste in Settings → Test → Save

**Anthropic Claude (alternative):**
1. Go to [console.anthropic.com](https://console.anthropic.com)
2. Sign up → API Keys → Create Key

### 3. Use

1. Open the deployed URL on your phone
2. Allow camera & microphone permissions
3. Select a mode → tap **ANALYSE**
4. AI describes what it sees and speaks the result aloud

> **No API key?** The app runs in demo mode with simulated responses.

## 🧠 Supported AI Models

| Provider | Models | Cost |
|----------|--------|------|
| Google Gemini | `gemini-2.5-flash`, `gemini-2.5-flash-lite`, `gemini-2.0-flash-lite` | Free |
| Anthropic | `claude-sonnet-4-5`, `claude-haiku-4-5` | Credits required |

## 🛡️ Privacy

- API keys are stored **only in your browser's localStorage**
- Images are sent **directly** to the AI provider — no intermediary server
- **Zero backend** — the entire app is a single HTML file

## 📁 Project Structure

```
index.html    ← entire application (HTML + CSS + JS, single file)
README.md     ← this file
```

## ⚙️ Tech Stack

- Vanilla HTML/CSS/JS — no frameworks, no build step
- Google Gemini API / Anthropic Claude API (vision)
- Web Speech API (text-to-speech + voice commands)
- MediaDevices API (camera)

## 📜 License

MIT — use freely for accessibility projects and beyond.
