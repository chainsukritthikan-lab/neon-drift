# 🏎️ NEON DRIFT

An open-world 3D street drifting game that runs entirely in your browser — on PC and phone. Built with [Three.js](https://threejs.org/), no build step, no backend, no downloads.

**▶ Play it: open `index.html` via any static server, or the GitHub Pages URL of this repo.**

![genre](https://img.shields.io/badge/genre-arcade%20drift-ff2d78) ![engine](https://img.shields.io/badge/engine-three.js-00e5ff) ![platform](https://img.shields.io/badge/platform-web%20%7C%20mobile-a855f7)

## Features

- **3 open-world maps** — Neon City (midnight downtown with neon signs), Sunset Strip (palms + giant setting sun), Fog Harbor (containers, mist, water)
- **4 buyable cars** with distinct extruded-silhouette bodies and stats (Street GT, Banshee V8, Kaido 86, Spectre X)
- **Drift combo scoring** — slip-angle physics, ×1–×5 multiplier, bank-or-lose risk loop
- **Checkpoint RACE mode with levels** — beat the clock through green beams; each level adds checkpoints and tightens the timer
- **Economy** — earn ¤ from coins, combos, near-misses, missions and races; spend on Engine/Tires/Turbo upgrades and new cars
- **Nitro** charged by drifting; manual throttle, brake & reverse, U-turn button
- **Living city** — AI traffic, parked cars, crosswalks, billboards, street lamps
- **Synth audio engine** — music, engine, tire screech, SFX, all generated with Web Audio (zero audio files)
- **Mobile-first** — touch pads, safe-area layout; keyboard on PC (A/D steer, W gas, S brake, X nitro, R u-turn, Space handbrake)
- **Persistent save** — cash, cars, upgrades, race level, lifetime stats in localStorage

## Run locally

```bash
cd drift-game
python -m http.server 7000
# open http://localhost:7000  (phone: http://<your-pc-ip>:7000 on the same Wi-Fi)
```

## Structure

```
index.html   home / landing page
game.html    the entire game (scene, physics, AI, audio, UI)
lib/         vendored three.js (no CDN needed — works offline)
```

Made with Claude Code.
