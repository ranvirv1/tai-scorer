# Taiwanese Mahjong Trainers 麻將

Free, offline practice tools for 16-tile Taiwanese Mahjong.

**[Live site →](https://ranvirv1.github.io/tai-scorer/)**

## Modules

### 台 Hand Scorer (`/scorer/`)
Practice recognising scoring patterns (台) in completed winning hands. Each round shows
a hand with its context — seat/round wind, self-draw or discard, concealed or open. You
pick which scoring patterns apply; the app reveals the correct breakdown and total 台.
Beginner mode shows English names and pip counts; Coach mode shows each pattern's value
as you pick.

### 守 Defense Trainer (`/defense/`)
Practice reading an opponent's discards and called melds to choose the safest tile to
throw and avoid dealing in (放槍). Each round shows a threatening opponent holding a
real, concealed tenpai hand with an exact computed wait. Coach mode labels each tile's
danger before you choose.

## Tech notes

- **Static HTML files.** No backend, no build step, no API keys, zero API cost.
- All logic runs in the browser. Each engine self-tests on load.
- Installable and offline-capable via web manifests + service workers.

## Run locally

Open any `index.html` in a browser. For offline/PWA testing:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy with GitHub Pages

1. **Settings → Pages → Source: Deploy from a branch.**
2. Choose `main` and `/ (root)`, then Save.
3. Live at `https://<you>.github.io/tai-scorer/` within a minute.

## License

MIT — see `LICENSE`.
