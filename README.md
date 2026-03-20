# The Forge

**A daily writing trainer. Sharpen the work, keep the voice.**

The Forge analyzes your writing and surfaces specific, actionable improvement points — then puts you to work fixing them in your own words. It targets structure, clarity, sentence rhythm, and word choice without touching your voice or style.

---

## How it works

1. **Paste or upload** a draft (`.txt` or `.md`)
2. **Choose** how many points to address (3, 5, or 7)
3. **The Forge analyzes** your draft and surfaces specific flagged moments with explanation and a quoted excerpt from your actual text
4. **For each point**, you write a response passage demonstrating the principle — in your own voice
5. **Your response is evaluated** and you get specific feedback before moving on
6. **End of session**: a score, per-point feedback, and a pattern note
7. **History view**: evolving writer assessment, category stats, and a log of your last 20 sessions

---

## Setup

The Forge uses the [Anthropic API](https://www.anthropic.com) to power its analysis. You need your own API key.

1. Get an API key at [console.anthropic.com](https://console.anthropic.com)
2. Open The Forge — you'll be prompted to enter your key on first launch
3. Your key is stored only in your browser's `localStorage` and sent only to `api.anthropic.com`

**Your API key is yours.** No one else can use your credits. Each session makes roughly 7–9 API calls (draft analysis + per-point evaluation + session summary + assessment update).

---

## Live app

**[https://uncle-jasper.github.io/forge/](https://uncle-jasper.github.io/forge/)**

---

## Installing as a PWA

Open the live app in your browser, then:

- **iOS**: Safari → Share → Add to Home Screen
- **Android**: Chrome → menu → Add to Home Screen
- **Desktop**: Chrome/Edge → install icon in the address bar

Each user is prompted for their own Anthropic API key on first launch. No one shares credits.

---

## Self-hosting

1. Fork [uncle-jasper/forge](https://github.com/uncle-jasper/forge)
2. Go to **Settings → Pages**
3. Set source to **Deploy from a branch** → `main` → `/ (root)`
4. Your fork will be live at `https://yourusername.github.io/forge/`

---

## Files

```
index.html       — the entire app (single file)
manifest.json    — PWA metadata
sw.js            — service worker (offline shell caching)
icons/           — app icons in 8 sizes + favicon + Apple touch icon
```

---

## Focus areas

| Area | What it targets |
|---|---|
| Structure & Flow | Logical progression, transitions, paragraph organization |
| Clarity & Concision | Vague language, hedging, over-explanation |
| Sentence Rhythm | Monotonous length, run-ons, choppiness |
| Word Choice | Weak verbs, filler words, imprecision |

---

## Privacy

- Your writing is sent to `api.anthropic.com` for analysis. It is subject to [Anthropic's privacy policy](https://www.anthropic.com/privacy).
- Your API key and session history are stored only in your browser's `localStorage`. Nothing is stored on any server.

---

## Version

**v1.0.0** — Initial release

---

*Vibe coded by Dan · © 2026*
