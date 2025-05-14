````markdown
# 🍩 Three.js “Donut Text” Playground

A small interactive Three.js demo that:

- Renders a 3D “Hello, Three.js !” mat‑cap text  
- Scatters hundreds of rotating “donuts” around it  
- Supports mouse orbit controls, responsive resize, fullscreen toggle, and a debug GUI  

---

## 🚀 Features

- **3D Text**  
  - Loaded via `FontLoader` + `TextGeometry`  
  - Centered pivot, customizable bevel, size, depth  
  - Uses a MatCap texture for shading  
- **Hundreds of Donuts**  
  - Shared `TorusGeometry` + `MeshMatcapMaterial` for performance  
  - Random position, rotation, and scale (within camera view)  
- **OrbitControls**  
  - Mouse/touch drag to rotate the camera  
  - Inertia (“damping”) for smooth motion  
- **Responsive & Fullscreen**  
  - Canvas auto‑resizes on window `resize`  
  - Double‑click to toggle fullscreen  
- **Debug GUI**  
  - Press `H` to hide/show the lil‑GUI panel  
  - (Ready for adding sliders to tweak material, lighting, donut count, etc.)

---

## 🛠️ Technologies

- [Three.js](https://threejs.org) r152  
- `lil-gui` for on‑screen controls  
- `gsap` for timeline‐based animations  
- Vite or your favorite bundler to serve ES modules  

---

## 📦 Installation

1. **Clone this repo**  
   ```bash
   git clone https://github.com/your‑username/threejs‑donut‑text.git
   cd threejs‑donut‑text
````

2. **Install dependencies**

   ```bash
   npm install
   ```
3. **Run a local dev server**

   ```bash
   npm run dev
   ```
4. **Open** `http://localhost:3000` (or whatever port Vite shows)

---

## 🔧 Usage

* **Orbit**: drag with mouse or touch
* **Zoom**: scroll wheel / pinch
* **Fullscreen**: double‑click canvas
* **Hide GUI**: press `H`

To tweak parameters (e.g. donut count, matcap, text string), edit the variables at the top of `main.js` or hook them up in the GUI folder.

---

## 📂 Project Structure

```
.
├── index.html
├── package.json
├── vite.config.js
├── src
│   ├── main.js      ← your Three.js scene code  
│   └── style.css    ← canvas & page styles  
└── static
    ├── fonts
    │   └── helvetiker_regular.typeface.json
    └── textures
        └── matcaps
            └── 8.png
```

---

## 🎯 Next Steps

* **InstancedMesh** for < 1000 donuts
* **Post‑processing**: bloom, grain, depth of field
* **Interactivity**: click to explode a donut, hover highlight
* **Mobile optimizations**: reduce geometry on small screens

Enjoy experimenting with Three.js, and feel free to ⭐ the repo if you find it useful!

