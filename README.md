# ARIA — Personal Intelligence Assistant

A privacy-first voice AI assistant. Runs as a PWA on your phone's home screen.
Powered by OpenAI Whisper (voice) + Anthropic Claude (AI brain).

---

## Quick Deploy to GitHub Pages

### 1. Create the repo
- Go to github.com → New repository
- Name it `aria` (will live at `yourusername.github.io/aria`)
- Set to **Public**
- Click Create

### 2. Upload files
Upload these files to the repo root:
- `index.html`
- `manifest.json`
- `sw.js`
- `icons/` folder (add icon-192.png and icon-512.png — see Icons section below)

### 3. Enable GitHub Pages
- Repo → Settings → Pages
- Source: Deploy from branch → main → / (root)
- Save — your app is live in ~60 seconds

---

## Icons

You need two icon files in an `icons/` folder:
- `icons/icon-192.png` — 192×192px
- `icons/icon-512.png` — 512×512px

Simple option: use any image editor or Canva to make a square ARIA logo.
ARIA branding suggestion: dark navy background (#060A14), "ARIA" in electric cyan (#00D4FF), Outfit Bold font.

---

## Install on iPhone (iOS)

1. Open Safari → go to `yourusername.github.io/aria`
2. Tap the Share button (box with arrow)
3. Tap **Add to Home Screen**
4. Name it ARIA → Add
5. Open from home screen — it runs fullscreen like a native app

**Important:** Always open from the home screen icon, not Safari directly,
for the best experience and reliable mic access.

---

## API Keys You Need

### OpenAI (Whisper — voice transcription)
1. Go to platform.openai.com
2. Create account → API Keys → Create new key
3. Cost: ~$0.006 per minute of audio. Very cheap for daily use.

### Anthropic (Claude — AI responses)
1. Go to console.anthropic.com
2. API Keys → Create key
3. Cost: ~$0.003 per 1K tokens. A typical conversation costs fractions of a penny.

Keys are stored locally on your device only — never on any server.

---

## First-Time Setup

On first launch, ARIA shows a setup screen:
- Enter your name and what you want to call your assistant
- Paste your OpenAI and Anthropic API keys
- Optionally add context about yourself (the more detail, the more personalised ARIA becomes)

---

## For Business / Multiple Users

Each user sets up their own keys and context. The app is fully configurable —
name, personality, context — all adjustable in Settings.

---

## File Structure

```
aria/
├── index.html       ← Main app (everything in one file)
├── manifest.json    ← PWA config
├── sw.js            ← Service worker (offline support)
└── icons/
    ├── icon-192.png
    └── icon-512.png
```

---

## Roadmap Ideas

- [ ] Google Calendar integration (read/create events by voice)
- [ ] PC agent connection (remote control via WebSocket)
- [ ] ElevenLabs TTS (higher quality voice)
- [ ] Wake word detection
- [ ] Conversation history export
- [ ] Multi-assistant profiles

---

Built by Rise & Strike · github.com/bradbarr
