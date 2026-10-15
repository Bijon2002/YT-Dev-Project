# Army Rush 3D — YouTube Playables Edition

[![Platform](https://img.shields.io/badge/Platform-YouTube%20Playables%20%7C%20Web-FF0000?style=for-the-badge&logo=youtube)](https://developers.google.com/youtube/gaming/playables)
[![Engine](https://img.shields.io/badge/3D%20Engine-Three.js%20(Self--Hosted)-000000?style=for-the-badge&logo=threedotjs)](https://threejs.org/)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](LICENSE)

An ultra-responsive, lightweight 3D crowd-runner and arcade battle game built specifically for **YouTube Playables**, mobile web, and modern desktop browsers.

---

## 🎮 Live Playable Demo

- **Hosted URL**: [https://bijoon.me/YT-Dev-Project/](https://bijoon.me/YT-Dev-Project/)
- **Alternate GitHub Pages**: [https://bijon2002.github.io/YT-Dev-Project/](https://bijon2002.github.io/YT-Dev-Project/)

---

## 🕹️ Gameplay & Features

- **5 Distinct Battle Zones**:
  1. *Zone 1: Verdant Plains* (Boss: Forest Warlord)
  2. *Zone 2: Sunset Canyon* (Boss: Canyon Titan)
  3. *Zone 3: Volcanic Fortress* (Boss: Nether Overlord)
  4. *Zone 4: Cyber Arena* (Boss: Mech Behemoth)
  5. *Zone 5: Celestial Apex* (Boss: Galactic Emperor)
- **Gates & Crowd Mechanics**:
  - Positive addition gates (`+5`, `+8`, `+12`)
  - Multiplier gates (`x2`, `x3`)
  - Red obstacles, hazard cones, and enemy squad formations
- **Procedural Sound Engine**:
  - 100% synthesized sound effects powered by the **HTML5 Web Audio API** (zero MP3/WAV assets to download, zero latency).
- **Armory Upgrades & Meta-Progression**:
  - Collect gold coins on the battlefield.
  - Upgrade **Starting Squad Size**, **Troop Firepower**, and **Agility / Movement Speed**.
- **Juice & Visual Polish**:
  - Particle bursts on gate breakthroughs and soldier defeats.
  - Dynamic camera shake on damage and boss hits.
  - Floating combo notifications and dynamic boss health bars.

---

## 🚀 YouTube Playables Compliance

This repository satisfies all Google YouTube Playables developer specifications:

| Requirement | Implementation Status |
| :--- | :--- |
| **SDK Integration** | `<script src="https://www.youtube.com/game_api/v1"></script>` loaded in `<head>`. |
| **Lifecycle Hooks** | `ytgame.game.firstFrameReady()` & `ytgame.game.gameReady()` implemented. |
| **Audio Compliance** | `ytgame.system.isAudioEnabled()` and `ytgame.system.onAudioEnabledChange(...)` synchronized. |
| **Pause/Resume** | `ytgame.system.onPause()` & `ytgame.system.onResume()` supported. |
| **Cloud Save / Scores** | `ytgame.game.saveData()` / `loadData()` & `ytgame.engagement.sendScore()`. |
| **No External CDNs** | Three.js (`three.module.js`) is completely self-hosted locally in `/js`. |
| **Zero Heavy WASM** | Instant startup (<400ms) with a total bundle size of ~1.3MB uncompressed. |

---

## 🛠️ Tech Stack Evaluation

### Why Three.js + Vanilla/Modern Web is Optimal for YouTube Playables:
- **Instant Cold Starts**: Unity or Godot Web exports require 15MB–40MB WASM binaries that take 8–15 seconds to initialize on mobile connections. Three.js initializes in milliseconds.
- **Memory Footprint**: Extremely low RAM usage, preventing mobile browser and iOS Safari tab crashes inside YouTube's iframe sandbox.
- **Asset-Free Audio**: Procedural sound synthesis eliminates network requests for audio files.

---

## ⌨️ Controls

- **Desktop**:
  - `A` / `D` or `←` / `→` to steer the squad.
- **Mobile**:
  - Drag left or right anywhere on the touchscreen.
- **Sound Toggle**:
  - Click the **Audio 🔊** pill in the top-right corner or use YouTube's platform sound toggle.

---

## 💻 Local Development

Run any standard local HTTP server in the repository root:

```bash
# Python
python -m http.server 8000

# Node / npx
npx serve .
```

Open `http://localhost:8000` in your browser.
