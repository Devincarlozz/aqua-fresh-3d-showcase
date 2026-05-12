# 🌊 Aqua Fresh 3D Showcase

[![Live Demo](https://img.shields.io/badge/Live%20Demo-View%20Now-00C7B7?style=for-the-badge&logo=cloudflare)](https://aqua-fresh-3d-showcase2.pages.dev/)
[![Built with Three.js](https://img.shields.io/badge/Three.js-Black?style=for-the-badge&logo=three.js&logoColor=white)](#)
[![Animated with GSAP](https://img.shields.io/badge/GSAP-88CE02?style=for-the-badge&logo=greensock&logoColor=white)](#)

A high-performance, fully interactive 3D product showcase built for the browser. Why build flat websites when you can build experiences? 

Experience the fluid 3D physics, cinematic crossfades, and highly optimized WebGL rendering natively on your desktop or mobile device.

---

## ✨ Features

- **Interactive 3D Physics:** Real-time fluid floating and mouse-tracking rotations using pure `Three.js`.
- **Cinematic Transitions:** Buttery-smooth, staggering fly-in typography and 360-degree can flips powered by `GSAP`.
- **Hyper-Optimized:** Built with raw Vanilla JavaScript and WebGL. No heavy frameworks. Loads instantly.
- **Responsive Layout:** Dynamically scales field-of-view and UI elements to look perfect on both ultra-wide monitors and small mobile screens.
- **Glassmorphism UI:** Features a sleek, modern, frosted-glass navigation bar and dynamic emoji icons.

---

## 🚀 Live Demo

Experience the live deployment hosted on Cloudflare Pages:
👉 **[Launch Aqua Fresh 3D](https://aqua-fresh-3d-showcase2.pages.dev/)**

---

## 🛠️ Technologies Used

- **HTML5 & CSS3:** For the structural layout, typography (`Anton` & `Outfit` fonts), and absolute positioning.
- **Vanilla JavaScript:** For application state, event handling (touch/wheel/mouse), and logic.
- **[Three.js (r128)](https://threejs.org/):** Powers the 3D WebGL scene, lighting (`SpotLight`, `DirectionalLight`), and materials (`MeshPhysicalMaterial`).
- **[GSAP (3.12.2)](https://greensock.com/gsap/):** Handles all complex timeline animations, easing, and stagger effects.

---

## 💡 How It Works

1. **The 3D Can:** The primary focal point is a procedurally generated `CylinderGeometry` with `TorusGeometry` rims. It uses `MeshPhysicalMaterial` with a high clearcoat to simulate real aluminum reflection.
2. **Dynamic Textures:** When a user scrolls or swipes, the `TextureLoader` dynamically swaps the diffuse map on the cylinder while it spins, creating a seamless flavor transition.
3. **Event Listeners:** The application listens for `wheel` (desktop scroll) and `touchstart`/`touchmove` (mobile swipe) to trigger the `changeDrink()` function, which orchestrates the complex GSAP timeline.

---

## 👨‍💻 Local Development

Want to run it locally or tweak the code? It's incredibly simple since there is no build step!

1. Clone the repository:
   ```bash
   git clone https://github.com/Devincarlozz/aqua-fresh-3d-showcase.git
   ```
2. Open the directory.
3. Because of WebGL CORS restrictions, you cannot just double click `index.html`. You need to run it through a local server. If you have VS Code, just use the **Live Server** extension, or run:
   ```bash
   npx serve .
   ```
4. Open your browser and enjoy!

---
*Built at 3 AM. If it breaks, it’s a feature. 🤝💻*
