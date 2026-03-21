# Gesture-Controlled 3D Particle System 🌌
An interactive, AI-powered 3D visualization that bridges the gap between physical movement and digital art. This project uses **MediaPipe** for real-time computer vision and **Three.js** for high-performance 3D rendering to create a touchless user interface.
## 🚀 Key Features
* **Real-time Hand Tracking:** Utilizes MediaPipe's palm detection to track 21 hand landmarks directly in the browser.
* **Dynamic Morphing:** Smoothly transitions 10,000+ particles between complex mathematical shapes (Sphere, Heart, Saturn, and Flower).
* **Intuitive Gesture Controls:**
    * **Scale:** Pinch **Index + Thumb** to expand or contract the system.
    * **Color Shift:** Pinch **Middle + Thumb** to cycle through vibrant hex colors.
    * **Shape Morph:** Pinch **Pinky + Thumb** to trigger a transition to the next geometric template.
* **Performance Optimized:** Uses `BufferGeometry` and `AdditiveBlending` to maintain high frame rates even with thousands of active vertices.
## 🛠️ Technical Stack
* **Frontend:** HTML5
* **3D Engine:** [Three.js](https://threejs.org/)
* **AI/ML:** [Google MediaPipe Hands](https://google.github.io/mediapipe/solutions/hands.html)
* **Math:** Parametric equations for complex 3D shape generation.
## 📐 Mathematical Templates
The morphing effect transitions particles between target coordinates calculated using specific equations:
* **Heart Shape:** $x = 16\sin^3(t)$, $y = 13\cos(t) - 5\cos(2t) - 2\cos(3t) - \cos(4t)$.
* **Flower (Rose Curve):** $r = a \sin(k\theta)$ where $k=5$ for a 5-petal effect.
* **Saturn:** A hybrid system consisting of a spherical core and a flat disc calculated via trigonometric circle constants.
## 📖 How to Run
1.  Clone the repository:
    ```bash
    git clone [https://github.com/your-username/gesture-3d-particles.git](https://github.com/your-username/gesture-3d-particles.git)
    ```
2.  Open `3dai.html` in any modern web browser.
3.  Ensure your webcam is enabled and stay within the frame.
> **Privacy Note:** This project processes all camera data locally on your device. No images or video feeds are sent to any external servers or stored.
## ✨ About the Developer
I am a **Computer Science and Engineering (CSE)** student with a deep interest in **Web Development** and **Cybersecurity**. This project explores how "Secure by Design" principles can be applied to emerging AI-driven user interfaces.
---
Developed by **Mayank Parashar** 
