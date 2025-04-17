# Space Shooter WebGL

> **Asteroids‑style browser shooter built with vanilla JavaScript and raw WebGL.**

<div align="center">
  <img src="https://github.com/user-attachments/assets/5455c5f7-4123-4fc5-9a14-065434bbb91a"
       alt="Gameplay GIF" width="900"/>
</div>


---

## 🎯 Why I built it

- **Learn WebGL by hand** – write GLSL shaders, manage buffers, and think in clip‑space without helper libraries.
- **Experiment with AI‑assisted coding** – used the Cursor editor plus ChatGPT for quick prototyping and refactors.

## 🚀 Gameplay

- 360° rotation with thrust‑based movement and inertia
- Screen‑wrapping edges for that classic arcade feel
- Laser shots with cooldown and limited lifetime
- Dynamic asteroid field: new rocks spawn as you destroy them, gradually ramping up difficulty
- Particle‑based explosion effects
- Score counter and GAME OVER screen with a **Play Again** button

### Controls

| Action       | Keys                              |
| ------------ | --------------------------------- |
| Thrust       | `W` / `↑`                         |
| Rotate left  | `A` / `←`                         |
| Rotate right | `D` / `→`                         |
| Fire laser   | `Space`                           |
| Restart      | Click **Play Again** when you die |

## 🛠 Tech stack

| Layer      | Choice                     | Notes                                                       |
| ---------- | -------------------------- | ----------------------------------------------------------- |
| Language   | JavaScript (ES2020)        | Plain browser APIs                                          |
| Rendering  | Raw WebGL 1.0              | Custom vertex & fragment shaders                            |
| Build tool | _None_ (any static server) | Shader files are fetched at runtime — browsers require HTTP |
| AI assist  | Cursor IDE + ChatGPT       | Refactors, shader tweaks                                    |

## 🏃 Getting started

> **Note:** the game fetches shader files at runtime, so most browsers block it when opened via `file://`. You’ll need to serve the folder through any static HTTP server.

Clone the repository

```bash
git clone https://github.com/ramonmello/space-shooter-webgl
cd space-shooter-webgl
```

Launch a tiny static server (Python 3.x)

```bash
python -m http.server 8000
```

Alternative (Node.js, if installed)

```bash
npx serve -l 8000
```

Then visit `http://localhost:8000` in your browser and start blasting.

## 🗺 Roadmap

- [ ] Sound effects & background music
- [ ] Mobile touch controls
- [ ] Power‑ups (shield, spread shot, mega bomb)
- [ ] Leaderboard via localStorage or a simple backend
- [ ] Migrate rendering pipeline to **WebGL 2.0**
- [ ] WebGPU prototype branch 🤔

## 🤝 Contributing

Found a bug or have an idea? Open an issue or PR – let’s talk!

---

> Made with caffeine, curiosity, and way too many shattered asteroids. Enjoy! 🚀
