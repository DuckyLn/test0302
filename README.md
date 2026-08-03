# 🌸 桜通り — Sakura Street

An explorable **anime-style 3D Japanese suburban street** built entirely with [Three.js](https://threejs.org/). The scene is rendered in a **3D-to-2D cel-shaded** aesthetic, evoking the look and feel of hand-drawn anime backgrounds.

![Three.js](https://img.shields.io/badge/Three.js-r163-blue?logo=threedotjs)
![License](https://img.shields.io/badge/License-MIT-green)
![HTML5](https://img.shields.io/badge/HTML5-Single%20File-orange?logo=html5)

## ✨ Features

### Visual Style
- **Cel shading** — 3-band toon materials for a hand-drawn anime look
- **Post-processing outlines** — Depth-based Sobel edge detection for clean dark outlines
- **Anime lighting** — Warm sunlight (`#FFF5E0`) + cool purple ambient (`#8B7FAA`)
- **Pastel gradient sky** with sun glow effect
- **Vignette & warm color grading** in post-processing

### Scene Elements

| Category | Details |
|---|---|
| 🛤️ **Railway** | Tracks, ties, gravel bed, stone retaining wall, guardrails |
| 🚆 **Train** | 3-car stylized commuter train, passes through every ~22 seconds |
| 🚧 **Crossing** | Animated barriers, flashing warning lights, X sign, road markings |
| 🌸 **Cherry Blossoms** | 6 sakura trees with clustered pink canopies + 350 falling petals |
| 🏘️ **Buildings** | 10+ Japanese houses with hip roofs, windows, doors, fences |
| 🏪 **Shop** | Small local shop with red awning, noren curtain, warm interior light |
| 🥤 **Vending Machines** | Red + blue glowing machines with drink displays and point lights |
| ⚡ **Utility Poles** | Poles with cross-arms, insulators, transformers, sagging catenary wires |
| 🚲 **Props** | Bicycles, road mirrors, signs, potted plants, red mailbox, manholes, AC units, a cat 🐱 |

### Interaction
- **First-person exploration** with smooth movement
- **WASD / Arrow Keys** — Move
- **Mouse** — Look around
- **ESC** — Pause / unlock cursor

## 🚀 Getting Started

### Option 1: Local Server (Recommended)

```bash
# Clone the repo
git clone https://github.com/DuckyLn/test0302.git
cd test0302

# Serve locally (pick one)
npx serve .
# or
python -m http.server 8000
```

Then open **http://localhost:3000** (or `:8000`) in your browser.

### Option 2: Open Directly

Simply open `index.html` in a modern browser (Chrome, Edge, Firefox). The scene loads Three.js from a CDN, so an internet connection is required.

> **Note:** Some browsers may restrict ES module imports from `file://`. If the scene doesn't load, use a local server instead.

## 🛠️ Tech Stack

- **Three.js r163** — 3D rendering engine (loaded via CDN / ES modules)
- **Custom GLSL Shaders** — Sky gradient, post-processing outlines, vignette, color grading
- **MeshToonMaterial** — Cel-shaded materials with stepped gradient maps
- **InstancedMesh** — Efficient rendering of 350 cherry blossom petals
- **PointerLockControls** — First-person camera controls
- **Vanilla HTML/CSS/JS** — Single-file, zero build step, no dependencies to install

## 📁 Project Structure

```
test0302/
└── index.html    ← Everything in one file (~1500 lines)
```

All 3D geometry is **procedurally generated** using basic primitives (boxes, cylinders, spheres, cones). No external 3D models, textures, or image assets are used.

## 📄 License & Attribution

### This Project

This project is licensed under the **MIT License** — feel free to use, modify, and distribute.

### Third-Party

| Dependency | License | Usage |
|---|---|---|
| [Three.js](https://github.com/mrdoob/three.js/) | [MIT](https://github.com/mrdoob/three.js/blob/dev/LICENSE) | 3D rendering engine, loaded via CDN |

### Originality Statement

All source code in this project is **written from scratch**. No code, 3D models, textures, or assets were copied from any other project. The only external dependency is Three.js (MIT license), loaded from a public CDN. The anime-style visual approach (cel shading, toon materials, outline post-processing) is a common rendering technique and does not derive from any specific copyrighted work.

## 🙏 Acknowledgments

- [Three.js](https://threejs.org/) — The amazing 3D library that makes this possible
- Inspired by the aesthetic of Japanese anime backgrounds (Makoto Shinkai, Studio Ghibli)

---

Made with ❤️ and Three.js