# Army Rush 3D — YouTube Playables Master Edition

[![Platform](https://img.shields.io/badge/Platform-YouTube%20Playables%20%7C%20Web-FF0000?style=for-the-badge&logo=youtube)](https://developers.google.com/youtube/gaming/playables)
[![3D Engine](https://img.shields.io/badge/3D%20Engine-Three.js%20(Self--Hosted)-000000?style=for-the-badge&logo=threedotjs)](https://threejs.org/)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](LICENSE)

An arcade 3D squad-runner and boss-battler engineered for **YouTube Playables**, mobile web, and modern desktop browsers.

---

## 🎮 Live Playable Demo

- **Hosted Domain**: [http://bijoon.me/YT-Dev-Project/](http://bijoon.me/YT-Dev-Project/)
- **GitHub Pages Alternate**: [https://bijon2002.github.io/YT-Dev-Project/](https://bijon2002.github.io/YT-Dev-Project/)

---

## 🗺️ 10 Unique Battle Zones & Bosses

| Zone | Biome | Environment Props | Boss Encounter |
| :---: | :--- | :--- | :--- |
| **1** | **Verdant Plains** | Oak trees, boulders & rolling green meadows | **Forest Warlord** *(Giant War Club)* |
| **2** | **Sunset Canyon** | Saguaro cacti, red sandstone cliffs | **Canyon Titan** *(Twin Axes)* |
| **3** | **Frozen Tundra** | Snowdrifts, ice crystals, pine trees | **Frost Colossus** *(Ice Mace)* |
| **4** | **Volcanic Caldera** | Obsidian crags, magma spires | **Nether Overlord** *(Molten Greatsword)* |
| **5** | **Cyber Neon City** | Cyberpunk towers, data monoliths | **Mech Behemoth** *(Plasma Cannons)* |
| **6** | **Toxic Wasteland** | Radioactive sludge, biohazard containers | **Mutant Goliath** *(Acid Spitter)* |
| **7** | **Sunken Atlantis** | Deep ocean seabed, vibrant coral groves | **Leviathan King** *(Trident)* |
| **8** | **Golden Pharaoh** | Desert dunes, sandstone pyramids & obelisks | **Pharaoh Emperor** *(Sun Scepter)* |
| **9** | **Dark Void Nether** | Cosmic void purple, dark matter anomalies | **Void Reaver** *(Dark Scythe)* |
| **10** | **Celestial Apex** | Astral golden dawn, marble pillars & arches | **Galactic Sovereign** *(Dual Blades)* |

---

## ⚔️ Thrilling Gameplay Mechanics

- **Choice Split Decision Gates**:
  - High reward gates (`x2`, `+12`) versus safer small gains (`+4`).
  - Penalty gates (`-4`, `-6`) requiring quick steering evasions.
- **Dynamic Hazard Traps**:
  - **Oscillating Spiked Pendulums**: Massive spiked blades swinging across the track.
  - Spiked road cones and barricades.
- **Power-Ups**:
  - **Nitro Overdrive Pad**: Accelerates your army at supersonic speeds with temporary hazard invulnerability.
  - **Aegis Energy Shield**: Absorbs a lethal hazard impact without casualties.
  - **Gold Coin Rings**: Boost your bank to invest in permanent upgrades.
- **Boss Shockwaves & Enrage Mode**:
  - Bosses release expanding kinetic shockwaves that sweep through lanes.
  - Squads automatically return laser fire against the boss.
- **Zone Select Menu**:
  - Select and replay any of the 10 unlocked zones at any time from the HUD or main menu.

---

## 🔊 Procedural Audio Engine

- **Web Audio API Synthesis**: Sound effects are generated mathematically on-the-fly via oscillators.
- **Zero Audio Assets**: No MP3/OGG files to load; 0ms latency, zero bandwidth impact.
- **YouTube Playables Audio Sync**: Automatically respects YouTube's global mute/unmute events.

---

## 🛠️ YouTube Playables SDK Integration

- `<script src="https://www.youtube.com/game_api/v1"></script>` loaded at the root of `<head>`.
- `ytgame.game.firstFrameReady()` & `ytgame.game.gameReady()`.
- Lifecycle pause/resume handlers (`onPause`, `onResume`).
- High-score broadcasting (`ytgame.engagement.sendScore()`).
- Cloud game saves (`ytgame.game.saveData()` / `loadData()`).

---

## ⌨️ Controls

- **Desktop**: `A` / `D` or `←` / `→`
- **Mobile Touch**: Drag left or right anywhere on the screen
- **Audio**: Click the **Audio 🔊** button in the top HUD
- **Zone Select**: Click the **Zone 🗺️** button in the top HUD
