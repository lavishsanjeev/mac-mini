# Apple Mac mini - 3D Interactive Web Experience

A high-fidelity 3D website for the **Apple Mac mini (M4 & M4 Pro)**, featuring real-time **Three.js** 3D modeling, smooth **40-frame scroll-driven image sequence scrubbing**, an interactive **Mac mini Configurator**, and an Apple-grade **Bento Grid**.

Built strictly adhering to **Cupertino Industrial Design** principles and **[UI UX Pro Max](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)** design intelligence — completely free of generic AI neon glow effects.

---

## 🌟 Key Highlights

### 1. Interactive Three.js 3D Studio
- **Procedural PBR Model**: Anodized aluminum unibody chassis with accurate metalness, roughness, clearcoat, and room environment reflection mapping.
- **Finish Switcher**: Toggle between **Anodized Silver**, **Space Black**, and **Starlight Titanium** with smooth color and roughness transitions.
- **Interactive Exploded View**: Top unibody separates upward to reveal the high-density logic board, copper M4 Pro silicon heat spreader, and dual centrifugal cooling fan impellers.
- **3D Hotspot Pins**: Projected from 3D space with direct camera fly-to inspection for:
  - Front USB-C (10Gb/s) & 3.5mm Headphone Jack
  - Apple M4 Pro Silicon Architecture
  - Aerodynamic Dual-Path Cooling System
  - Rear Thunderbolt 5 (120Gb/s), HDMI 2.1, and 10Gb Ethernet
- **Studio Lighting Presets**: Switch between *Softbox Studio*, *Dramatic Rim Key*, and *Clean Minimalist*.
- **Camera Angles**: Instant smooth transitions for *360° Studio*, *Front I/O*, *Rear Ports*, *Top Architecture*, and *Exploded View*.

### 2. 40-Frame Canvas Scroll-Scrubbing ("Inside Teardown")
- **Hardware Teardown Scrubbing**: Utilizes all 40 user-provided frames (`ezgif-frame-001.jpg` to `ezgif-frame-040.jpg`).
- **Smooth Sub-frame Lerping**: Buttery smooth frame progression as you scroll through the 380vh section with high-DPI canvas scaling.
- **Synchronized Apple Storytelling**:
  - *Phase 1 (Frames 1–12)*: Microscopic 5×5-inch enclosure precision.
  - *Phase 2 (Frames 13–26)*: Apple Silicon M4 / M4 Pro architecture revealed.
  - *Phase 3 (Frames 27–40)*: Whisper-quiet dual-fan thermal aerodynamics.
- **Interactive Manual Scrubber**: Floating scrub bar with range slider, frame indicator (`01 / 40`), auto-play toggle, and frame-stepping controls.

### 3. Apple Bento Grid Performance Matrix
- **Interactive Benchmark Widget**: Toggle between *Multithreaded CPU*, *GPU Ray Tracing*, and *Apple Intelligence Neural Engine* with real-time animated comparative bar graphs.
- **Key Hardware Callouts**: Thunderbolt 5 bandwidth comparison (120Gb/s vs 40Gb/s), unified memory up to 64GB (273GB/s), and carbon-neutral sustainability milestones.

### 4. Mac mini Studio Configurator & Live Pricing
- **Chip Selection**: M4 (10-core CPU/GPU) vs M4 Pro (12-core or 14-core CPU, up to 20-core GPU).
- **Unified Memory**: 16GB, 24GB, 32GB, 48GB, or 64GB.
- **Storage**: 256GB, 512GB, 1TB, 2TB, or 4TB SSD.
- **Networking**: Gigabit vs 10 Gigabit Ethernet.
- **Live Pricing Engine**: Calculates real-time total price and Apple Card monthly installment breakdown.
- **Bag Modal Sheet**: Complete order preview with taxes, free two-day shipping, and simulated Apple Pay checkout.

### 5. Authentic Cupertino Aesthetics (Zero AI Glow)
- Authentic obsidian black (`#000000`, `#08080a`), hairline 1px borders (`rgba(255, 255, 255, 0.08)`), SF Pro typography, and realistic physical lighting.
- Optional tactile synthesized audio feedback (Web Audio API) with global mute switch in the navigation bar.

---

## 🚀 How to Run the Website

### Option A: Development Server (Vite)
```bash
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

### Option B: Production Preview
```bash
npm run build
npm run preview
```
Or serve the pre-built `dist/` directory with any static server:
```bash
python -m http.server 8080 --directory dist
```
Open [http://localhost:8080](http://localhost:8080).

---

## 📁 Project Structure

```
├── public/
│   ├── frames/             # All 40 teardown animation frames (ezgif-frame-001.jpg - 040.jpg)
│   └── video.mp4           # Teardown video source
├── src/
│   ├── scripts/
│   │   ├── three-scene.js      # Three.js 3D Mac mini studio, PBR materials & hotspots
│   │   ├── scroll-sequence.js  # 40-frame scroll-driven canvas scrubbing engine
│   │   ├── configurator.js     # Interactive Apple Mac mini configurator & pricing
│   │   ├── audio.js            # Synthesized Web Audio API tactile feedback
│   │   └── main.js             # App orchestration, Lucide icons & benchmarks
│   └── styles/
│       └── main.css            # Apple industrial design system & responsive styling
├── dist/                   # Production-ready built distribution
├── index.html              # Main landing page markup
├── package.json            # Node.js project configuration
└── vite.config.js          # Vite build and dev configuration
```
