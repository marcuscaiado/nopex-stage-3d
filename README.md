# NOpex 3D // Open-Air Hip-Hop Festival & Live Stage

A zero-cost, high-density 3D live concert environment running natively on GitHub Pages with dual WebGL + CSS3D rendering, synchronized YouTube pro-shot broadcasts, and anonymous peer-to-peer multiplayer crowds supporting up to 100 concurrent users via WebRTC / BitTorrent tracker signaling.

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Three.js](https://img.shields.io/badge/Three.js-r168-black.svg)
![P2P](https://img.shields.io/badge/P2P-Trystero_BitTorrent-green.svg)

---

## ⚡ Key Features

- **Dual-Engine Rendering:** Synchronized `THREE.WebGLRenderer` and `THREE.CSS3DRenderer` projection matrices for a massive 38m 16:9 concert screen bypassing browser CORS sandbox limitations.
- **Zero-Cost P2P Multi-User:** Serverless mesh networking via public BitTorrent trackers (`trystero/torrent`). Packed flat telemetry broadcast at 15 Hz with dead-reckoning lerp interpolation and automatic 5s GC cleanup.
- **Concert Lighting Rig:** 6 moving-head spotlights animated with Lissajous oscillatory curves, procedural 135 BPM audio pulse clock, volumetric additive beams, vibrating subwoofer cones, and periodic blinding strobes.
- **Brutalist Anonymous Avatars:** 100% anonymous (no text chat, no microphones, no nametags). Procedural low-poly humanoid rig with kinematics engine (Idle, Walk/Run, Hip-Hop Bounce, Trap Arms Hype, Jump pose, Head Nod).
- **Customization & Visor Shader:** Real-time 8-palette clothing selector, modular accessories (Cyber Visor, Cuban Link Chain, Studio Headphones), and active CRT scanline / chromatic aberration visor overlay.

---

## 🚀 Running Locally

You can serve the directory statically with any web server:

```bash
# Using Node / npx
npx serve . -p 5173

# Or Python
python -m http.server 5173
```

Then open `http://localhost:5173` in your browser.

---

## 🎮 Controls

| Action | Control |
|---|---|
| **Look / Orbit** | Click canvas to lock pointer / Mouse movement |
| **Move** | `W`, `A`, `S`, `D` or Arrow Keys |
| **Sprint** | Hold `Shift` |
| **Jump** | `Space` |
| **Idle Emote** | `1` |
| **Hip-Hop Bounce** | `2` |
| **Trap Arms Hype** | `3` |
| **Head Nod** | `4` |
| **Avatar Rig Config** | `C` or HUD Button |
| **Zoom In / Out** | Mouse Wheel |

---

## 🌐 Deploy to GitHub Pages

Push this repository to GitHub, navigate to **Settings > Pages**, and select `Deploy from a branch > main / root`. No build step or server required!
