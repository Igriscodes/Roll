# ROLL — Endless Runner

A high-speed endless runner built with Three.js. Dodge obstacles, collect coins, and let the AI pilot assist you — all in a single HTML file.

![5807796e4e96902f](https://github.com/user-attachments/assets/52bfbefd-51e6-4efa-8c3d-b7025f283c41)

## Play Now

Open `app.html` in any modern web browser. No server, build step, or installation required.

## How to Play

- **←** / **A** — Move left  
- **→** / **D** — Move right  
- **Tap left/right** (touch) — Mobile swipe control  
- **Goal** — Survive as long as possible, collect gold coins, and avoid barriers.

Your speed increases over time. The game ends when you hit an obstacle.

## AI Pilot

An **AI agent** runs in a separate Web Worker. It constantly evaluates the track ahead:

- Detects obstacles and coins up to 50 units forward.
- Avoids occupied lanes and chooses the safest path.
- Prioritizes collecting coins when safe.
- Can be overridden by manual input.

The AI’s thoughts are displayed in the top‑left corner.

## Features

- **Fully 3D** with shadows, dynamic lighting, and particle effects.
- **Procedurally generated chunks** with varied obstacle layouts (barriers, ramps, coins).
- **Smooth lane switching** with camera following.
- **Speed‑based difficulty** — faster speeds increase collision tolerance.
- **Trail effect** and screen shake for impact.

## Technical Details

- **Engine:** Three.js r128 (WebGL)
- **AI:** Web Worker thread for real‑time pathfinding
- **Architecture:** Single HTML file with embedded CSS, JS, and GLSL
- **Performance:** Shadow mapping, fog, and efficient object pooling for obstacles and coins

## License

[GNU Lesser General Public License v2.1](LICENSE) - Feel free to use and modify
