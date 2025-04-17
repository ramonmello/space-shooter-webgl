# Space Shooter WebGL

> **Asteroids‑style browser shooter built with vanilla JavaScript and raw WebGL.**

<div align="center">
  <!-- Replace with GIF or video once recorded -->
  <img src="docs/media/demo-placeholder.gif" alt="Gameplay recording" width="600"/>
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

| Layer      | Choice               | Notes                                      |
| ---------- | -------------------- | ------------------------------------------ |
| Language   | JavaScript (ES2020)  | Plain browser APIs                         |
| Rendering  | Raw WebGL 1.0        | Custom vertex & fragment shaders           |
| Build tool | _None_               | Just open `index.html` or serve statically |
| AI assist  | Cursor IDE + ChatGPT | Refactors, shader tweaks                   |

## 🏃 Getting started

```bash
# Clone
git clone https://github.com/ramonmello/space-shooter-webgl
cd space-shooter-webgl

# Easy: open directly in a modern browser
open index.html

# Or serve with a tiny static server (recommended)
python -m http.server 8000
```

Then visit `http://localhost:8000` and start blasting.

## 🗺 Roadmap

- [ ] Sound effects & background music
- [ ] Power‑ups (shield, spread shot, mega bomb)
- [ ] Leaderboard via localStorage or a simple backend
- [ ] WebGPU prototype branch 🤔

## 🤝 Contributing

Found a bug or have an idea? Open an issue or PR – let’s talk!

---

> Made with caffeine, curiosity, and way too many shattered asteroids. Enjoy! 🚀
