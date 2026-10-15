# Army Rush 3D

A playable 3D browser prototype: collect troops, grow your squad, dodge hazards, fight enemy formations, and defeat the final boss.

## Run it
This project loads Three.js from jsDelivr, so internet access is required.

### Option A: Python local server
1. Extract the ZIP.
2. Open PowerShell in the `army-rush-3d` folder.
3. Run:
   `py -m http.server 8000`
4. Open `http://localhost:8000`.

### Option B: VS Code
Open the folder and use the Live Server extension on `index.html`.

## Controls
- Desktop: A/D or Left/Right arrows.
- Mobile: drag left/right on the screen.
- Click Start Mission to begin. After victory or defeat, use Retry/Play Again.

## Prototype notes
- Built with Three.js and WebGL.
- Includes procedural low-poly 3D troops, terrain, pickups, hazards, enemy squads, score, and boss health.
- This is a prototype, not a certified YouTube Playable. Before submitting, test on target devices and implement the current Playables requirements and any requested SDK/integration.
- Three.js is loaded from a CDN; bundle/self-host dependencies if the publishing requirements or offline use require it.

Official docs: https://developers.google.com/youtube/gaming/playables
