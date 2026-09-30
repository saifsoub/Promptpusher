# Promptpusher

Standalone prompt-driven apps, distributed as ready-to-unzip archives.

## Contents

| File | App |
|---|---|
| `lyria-alarm-clock.zip` | **Lyria Alarm Clock** — an AI alarm clock that composes a unique song every morning from your agenda, the weather, and your location |

## Lyria Alarm Clock

Built with React 19, TypeScript, Vite, and the Google Gen AI SDK. It combines three models:

| Model | Role |
|---|---|
| `gemini-3-flash-preview` | Turns your agenda, local weather, and location into a musical brief |
| `lyria-3-pro-preview` | Composes the song from that brief |
| `gemini-2.5-flash-preview-tts` | Renders the spoken layer |

### Run it

```bash
unzip lyria-alarm-clock.zip -d lyria-alarm-clock
cd lyria-alarm-clock
npm install
echo "GEMINI_API_KEY=your-key" > .env.local
npm run dev
```

Requires Node.js and a Google AI Studio API key. The app requests geolocation permission to
personalise the song.

## Layout

Each app ships as a single zip so it can be downloaded and run without cloning anything.
