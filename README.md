# Taiwanese Mahjong — 台 Hand Scorer

A browser-based practice tool for recognising scoring patterns (台) in completed
16-tile Taiwanese Mahjong winning hands.

## What it is

Each round shows a winning hand with its context — seat wind, round wind, self-draw
or discard, concealed or open. You pick which scoring patterns apply; the app reveals
the correct breakdown and total 台 count. Beginner mode shows English names and pip
counts; Coach mode shows each pattern's value as you pick.

The full 台 reference table is built into the app. Patterns marked with a warning
genuinely vary between house rules — the app uses one common, consistent table.

## Tech notes

- **A single static HTML file.** No backend, no build step, no API keys, zero API cost.
- All logic runs in the browser. The engine self-tests on load.
- Installable and offline-capable via a web manifest + service worker.

## Run locally

Open `index.html` in a browser. For offline/PWA testing:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy with GitHub Pages

1. **Settings → Pages → Source: Deploy from a branch.**
2. Choose `main` and `/ (root)`, then Save.
3. Live at `https://ranvirv1.github.io/tai-scorer/` within a minute.

## License

MIT — see `LICENSE`.
