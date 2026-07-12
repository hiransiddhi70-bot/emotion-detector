# 🎭 Day 17: Local Face Emotion Detector (#20day20ai)

A lightweight, zero-backend, client-side web application that detects human facial expressions in real-time. Built entirely in a single HTML file using **face-api.js**, this project runs deep learning models straight inside your browser or mobile phone—no API keys or server deployments required.

## ✨ Features
- **100% Client-Side:** Inference runs entirely locally via WebGL/WASM. Your camera feed never leaves your device (Complete Privacy).
- **Mobile First:** Designed with a clean, responsive dark-mode UI optimized for mobile viewports.
- **Zero Configuration:** Single file architecture (`index.html`) with absolute CDN dependencies—no `npm install` or build tools needed.

## 🛠️ Tech Stack
- **Frontend:** Semantic HTML5, Vanilla JavaScript (ES6+), and modern CSS Custom Properties.
- **AI/ML Engine:** `face-api.js` (Wrapper built on top of TensorFlow.js core) loading a pre-trained `TinyFaceDetector` and `FaceExpressionNet` graph.

## 🚀 How to Run & Deploy

### Option A: Quick Mobile Deployment (GitHub Pages)
1. Create a new repository on GitHub named `20day20ai-day17-emotion-detector`.
2. Commit the `index.html` file to the root of the repository.
3. Head to **Settings** > **Pages**. Under "Build and deployment", set the source to the `main` or `master` branch and hit **Save**.
4. Access the live link on your mobile browser (Ensure you load it over `https://` as mobile browsers require secure contexts to grant camera permissions).

### Option B: Local Development
Because browsers block camera access on flat `file://` protocols due to strict CORS security parameters, you must host it on a local environment:
- If using VS Code, right-click `index.html` and click **Open with Live Server**.
- Alternatively, spin up a quick python instance in your terminal: `python -m http.server 8000`.
- 
