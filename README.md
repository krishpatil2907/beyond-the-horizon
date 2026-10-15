# 🌌 Beyond the Horizon — An Interactive Journey
### Techfest IIT Bombay Campus Ambassador Showcase

> *"The horizon is not a boundary. It is an invitation to redefine what's possible."*

A responsive, high-performance **Interactive Parallax Scrolling Website** built for the **Techfest IIT Bombay Campus Ambassador** creative challenge. Engineered with multi-layered depth, SVG vectors, procedural particle simulations, dynamic HUD telemetry, and client-side procedural ambient sound synthesis via the Web Audio API.

---

## 🚀 Live Demo & Quick Start

### 1. Requirements
- **Node.js**: v18.0.0 or later (v20+ recommended)
- **Package Manager**: npm, pnpm, or yarn

### 2. Run Locally
```bash
# Navigate to project folder
cd beyond-the-horizon

# Install dependencies
npm install --legacy-peer-deps

# Start Vite Development Server
npm run dev
```
Open **[http://127.0.0.1:5173/](http://127.0.0.1:5173/)** in any modern web browser.

### 3. Build for Production
```bash
npm run build
npm run preview
```

---

## 🗺️ The 6 Cinematic Parallax Environments

| Section | Environment | Depth Planes & Key Features |
|---|---|---|
| **01. Orbit** | **Cosmic Universe (Hero)** | Dynamic Starfield Canvas (twinkles & shooting stars), multi-plane gas giant with rings, orbital telemetry beacon, 3D mouse parallax tilt, and scroll-down indicator. |
| **02. Summit** | **Stratosphere Divide** | Aurora Borealis glowing gradient curtains, distant frosted peaks, mid-ground cybernetic mountain conduits, volumetric creeping fog, and interactive altitude telemetry cards (8,848m, -48.5°C). |
| **03. Biodome** | **Bioluminescent Cradle** | Sun-shaft god rays, ancient bio-trees with glowing xylem veins, 75+ interactive bioluminescent spore particles responding to cursor proximity, and interactive "Transmit Bio-Harmonic Pulse" button. |
| **04. Abyss** | **The Hadal Trench** | Oceanic light caustics, floating bioluminescent jellyfish with undulating tentacles, dynamic rising bubbles, real-time depth meter (-800m to -10,928m), and interactive "Transmit Sonar Ping" acoustic wave. |
| **05. Nexus** | **Synapse Metropolis (Neo-Bombay 2099)** | Cyberpunk megalopolis skyline, illuminated megatowers with warning beacons, multi-level skyways with streaming aerial vehicle light-trails, and interactive observation skydeck telemetry modules. |
| **06. Singularity** | **The Horizon Singularity** | Celestial ascension portal with concentric spinning energy rings, closing manifesto, Techfest Campus Ambassador verified card, "Explore Again" warp scroll, and "Initiate Transmission" modal with confetti explosion. |

---

## 🎮 Interactive Features & Controls

1. **Dual-Layer Scroll Progress Bar**:
   - Top horizontal neon gradient progress bar (0% to 100%).
   - Right-side vertical floating waypoint tracker on desktop showing live sync percentage, interactive navigation jump nodes, and tooltips.
2. **Procedural Web Audio API Ambient Synthesizer**:
   - Zero external audio files or network latency. Pure client-side harmonic soundscapes that shift acoustic timbre and resonant frequencies as you move through each environment.
   - Built-in audio controls in the navigation bar with an animated live indicator.
3. **Custom Magnetic Fluid Cursor**:
   - Dual-ring follower with lerp interpolation.
   - Automatically adapts colors to the current environment and magnetizes to interactive buttons.
   - Intelligently disabled on touch screens and under `prefers-reduced-motion: reduce`.
4. **Dynamic Depth Gauge**:
   - Automatically calculates virtual oceanic depth (-800m down to -10,928m Mariana Trench level) and hydrostatic pressure in real time during scroll.
5. **Interactive Sonar Ping**:
   - Radiates an acoustic shockwave ring across the abyss and emits a synthesized submarine sonar ping.
6. **"Explore Again" Warp Scroll**:
   - Smoothly glides back to the summit of the experience with a single click.
7. **Interactive Satellite Transmission Modal**:
   - Triggers celebratory particle confetti and displays copyable Techfest mission dispatch coordinates.

---

## 🛠️ Architecture & Tech Stack

- **Framework**: React 19 + Vite 8
- **Icons**: Lucide React
- **Audio Engine**: Custom Web Audio API oscillator bank & biquad resonance filter
- **Visuals**: SVG Vector landscapes, Canvas generative physics, and CSS Glassmorphism
- **Performance**:
  - `transform: translate3d` hardware acceleration
  - `requestAnimationFrame` throttled scroll listener
  - Compositor-thread rendering (`opacity`, `transform`)
  - No broken external image URLs — all artwork rendered via crisp scalable vectors and procedural canvas
- **Accessibility**:
  - Respects `@media (prefers-reduced-motion: reduce)`
  - Full keyboard navigation and ARIA tags

---

## 🚢 Deployment Instructions

### Deploy to Vercel (Recommended)
1. Push this repository to GitHub.
2. Go to **[vercel.com](https://vercel.com/)** and click **"Add New Project"**.
3. Import your GitHub repository.
4. Settings:
   - **Framework Preset**: `Vite`
   - **Build Command**: `npm run build`
   - **Output Directory**: `dist`
   - **Install Command**: `npm install --legacy-peer-deps`
5. Click **Deploy**.

### Deploy to Netlify
1. Create a `netlify.toml` file in the root:
```toml
[build]
  command = "npm run build"
  publish = "dist"
```
2. Link your repository on **[netlify.com](https://netlify.com/)** and click **Deploy Site**.

---

## 🏆 Techfest IIT Bombay Campus Ambassador Attribution
- **Task**: Interactive Parallax Scrolling Website Showcase
- **Theme**: *Beyond the Horizon — An Interactive Journey*
- **Festival**: Techfest, IIT Bombay (Asia's Largest Science & Technology Festival)
- **Year**: 2026-2027
