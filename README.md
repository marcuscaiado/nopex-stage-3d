# NOpex 3D // Open-Air Hip-Hop Festival & Live Stage

A zero-cost, high-density 3D live hip-hop festival and concert environment running natively on GitHub Pages with dual WebGL + CSS3D rendering, continuous 24/7 Drake, Future, and Lil Baby live concert performances, 35 autonomous festival NPCs, Hallucinate-style controls, and anonymous peer-to-peer multiplayer crowds supporting up to 100 concurrent users via WebRTC / BitTorrent tracker signaling.

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Three.js](https://img.shields.io/badge/Three.js-r168-black.svg)
![P2P](https://img.shields.io/badge/P2P-Trystero_BitTorrent-green.svg)
![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-brightgreen.svg)

🌐 **Live Demo:** [https://marcuscaiado.github.io/nopex-stage-3d/](https://marcuscaiado.github.io/nopex-stage-3d/)

---

## ⚡ Key Features

- **Continuous 24/7 Live Stream:** Synchronized pro-shot concert sets from Drake (*It's All A Blur Tour MSG*), Future (*Rolling Loud*), and Lil Baby (*Rolling Loud California*).
- **Hallucinate "PLAY CONCERT" Button ("CANNOT STOP — ONLY PLAY"):** Dedicated glowing neon buttons on the top bar and dock that immediately start, play, and unmute concert audio at 100% volume with an active pause-guard watchdog.
- **35 Autonomous Festival NPCs:** Permanent AI crowd roaming the lush green lawn (gramado), dancing to 135 BPM trap beats (hip-hop bounce, trap hype arms, breakdance spins, head nods, wave hands), and moving between festival zones.
- **First-Person POV & Full Zoom:** Scrolling in with the mouse wheel smoothly transitions into an immersive first-person perspective, hiding local avatar obstruction and locking rotation to camera look direction.
- **Avatar Jump Action:** Pressing `Space` launches the avatar with vertical jump kinematics and poses.
- **Dual-Engine Rendering:** Synchronized `THREE.WebGLRenderer` and `THREE.CSS3DRenderer` projection matrices for a massive 38m 16:9 concert screen bypassing browser sandbox restrictions.
- **Zero-Cost P2P Multi-User:** Serverless mesh networking via public BitTorrent trackers (`trystero/torrent`). Packed flat telemetry broadcast at 15 Hz with dead-reckoning lerp interpolation and automatic 5s peer GC.
- **Concert Lighting Rig:** 6 moving-head spotlights with Lissajous oscillatory curves, volumetric additive beams, vibrating subwoofer cones, and stadium floodlight towers.
- **In-World 3D Features:** 3D Schedule Wall displaying set times and 3D Polaroid Photo Wall capturing snapshots (`F`).

---

## 🎮 Controls & Shortcuts

| Action | Key / Control |
|---|---|
| **Play Concert [Cannot Stop]** | `[PLAY CONCERT]` Button / `[P]` / Dock Pill |
| **Move Avatar** | `W`, `A`, `S`, `D` or Arrow Keys |
| **Jump** | `Space` |
| **Look / Mouse Look** | Click canvas to lock pointer / Move Mouse |
| **First Person / Zoom** | Mouse Wheel (Scroll In = 1st Person, Scroll Out = 3rd Person) |
| **Switch Camera Mode** | `T` (Chase, 1st-Person, Front Stage VIP, DJ Deck) |
| **Breakdance Power Move** | `Y` |
| **Wave Hands Emote** | `V` |
| **Bounce / Jetpack Boost** | `B` |
| **Party Bubbles** | `C` |
| **CO2 Foam Cannon** | `N` |
| **Photo Snapshot -> Wall** | `F` |
| **Cyber Sunglasses / Visor** | `G` |
| **In-Game Chat / Speak** | `Enter` |
| **Avatar Rig Customizer** | `Tab` |
| **Hair Color Cycle** | `7` / `8` |
| **Skin Tone Cycle** | `9` / `0` |
| **Top Wear Color Cycle** | `J` / `K` |
| **Bottom Wear Color Cycle**| `M` / `,` |
| **Dance Move Cycle** | `L` / `;` |
| **Help Modal** | `H` or `?` |

---

Markdown
## 🚀 Running Locally

Because this project relies on ES Modules and WebGL/Three.js assets, opening `index.html` directly via the file system (`file://`) will fail due to browser CORS policies. You must run it through a local HTTP server.

### Option 1: Node.js (Recommended)

Run directly using `npx` (requires Node.js installed):

```bash
npx serve . -l 8088
Option 2: Python
If you have Python installed, launch the built-in HTTP server:

Bash
# macOS / Linux
python3 -m http.server 8088

# Windows
python -m http.server 8088
After starting the server, open your browser and navigate to:

👉 http://localhost:8088
