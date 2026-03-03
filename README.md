# 🌍 KercMap: The Procedural Cartography Engine
> **Break the 4th wall of software: The Game is the Manual.**

![KercMap Header](https://capsule-render.vercel.app)

[![GitHub stars](https://img.shields.io)](https://github.com)
[![GitHub watchers](https://img.shields.io)](https://github.com)
[![License: MIT](https://img.shields.io)](https://opensource.org)

## 📍 Concept: "Executable Documentation"
Most engines hide their logic. **KercMap** puts it in the spotlight. 
- **Inspect-to-Learn:** Every pixel on the map is an entry point to the source code.
- **Dynamic Feedback:** Tweak the `erosion_factor` in the UI and watch the C++ WASM-module recalculate the world in real-time.

---

## 🛠️ The Tech Stack (Deep Dive)

### ⚙️ The Core (C++)
Located in `/src/core`. Responsible for high-load computations:
- **Tectonic Plates:** Euler rotation math for realistic continents.
- **Hydraulic Erosion:** Simulation of water carving canyons (simulated via 2D-arrays).
- **Fast Noise:** Custom SIMD-optimized Simplex noise.

### 🧠 Linguistic Module (Python)
Located in `/src/linguistics`. It's the "DNA" of your world:
- **Phoneme Seed:** Generates a unique alphabet for every save-file.
- **Toponymy:** Naming rivers and mountains based on surrounding biomes.

### 🎨 Web Renderer (TypeScript / Vite)
Located in `/src/frontend`. 
- **WebGL/Canvas:** Renders millions of tiles at 60 FPS.
- **Bridge:** Uses **WebAssembly (WASM)** to talk to the C++ core at native speed.

---

## 🗺️ Roadmap (The Future of KercMap)
- [ ] **Phase 1:** Core noise generation and basic TS-viewer. (Current)
- [ ] **Phase 2:** WASM integration for real-time C++ erosion.
- [ ] **Phase 3:** Python-based culture and dialect generator.
- [ ] **Phase 4:** Export to `.SVG` and `.OBJ` for 3D printing your worlds.

---

## 👨‍💻 Contributing
KercMap is built by the community. Check our [Issues](https://github.com) to find "Good First Issues".

1. **Fork** it.
2. **Feature** it.
3. **Star** it.

---

## 📜 Community & License
- **License:** [MIT](LICENSE)
- **Code of Conduct:** [Contributor Covenant](CODE_OF_CONDUCT.md)

> "Reality is just a simulation with bad documentation. KercMap fixes that."
