# Promptpusher — plain-language README

## What this is
A place to download small, ready-made AI apps as zip files. Unzip one and run it; there's no need to copy the whole project.

## Who it's for
Anyone who wants to try these apps on their own computer.

## What it does today
It currently holds one app.

**Lyria Alarm Clock** (`lyria-alarm-clock.zip`): an alarm clock that writes a new song for you every morning. It looks at your day's agenda, the local weather and where you are, then:
1. Google's Gemini AI turns those into a short description of the song.
2. Google's Lyria AI composes the music.
3. A Gemini voice adds a spoken part.

It asks for permission to use your location so it can personalise the song.

## How to run it
You need Node.js and a Google AI Studio key (free to request from Google).
```bash
unzip lyria-alarm-clock.zip -d lyria-alarm-clock
cd lyria-alarm-clock
npm install
echo "GEMINI_API_KEY=your-key" > .env.local
npm run dev
```

## Current status and known gaps
- One app so far.
- The Google AI models it uses are marked "preview", so they may change or stop working.

## Where things live
| File | What's in it |
|---|---|
| `lyria-alarm-clock.zip` | The alarm-clock app |
