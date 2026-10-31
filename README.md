# OVERDRIVE

<div align="center">

### NO BRAKES. NO LIMITS. JUST DRIVE.

A browser-based 3D driving game with endless highway survival, circuit racing, and local split-screen multiplayer.

![OVERDRIVE Garage](assets/garage.png)

[Game modes](#-game-modes) · [Screenshots](#-screenshots) · [Controls](#-controls) · [Run locally](#-getting-started)

</div>

---

## 🏁 About

**OVERDRIVE** is a 3D driving game built around two styles of driving: survive an endless three-lane highway by dodging traffic, or race around a circuit against AI opponents or another player on the same keyboard.

Customize your car, choose your challenge, and hit the road.

## 🎮 Game Modes

### Endless Traffic

Survive as long as possible on a three-lane highway.

- Traffic arrives in three lanes; avoid collisions to keep your run alive.
- Speed and distance increase as you survive.
- Choose **Chill**, **Normal**, or **Insane** traffic difficulty in the Garage.
- Your distance is your score, and your best run is saved in your browser.
- Touchscreen steering is supported: hold the left or right side of the screen.

### AI Race

Race against computer-controlled drivers on a circuit.

- Choose **1–5 AI opponents**.
- Set AI difficulty to **Easy**, **Normal**, or **Hard**.
- Choose a circuit and race length.
- View your position, lap, race timer, speed, drift distance, and a minimap.

### Buddy Race

Two players, one keyboard, split-screen racing.

- Local multiplayer with two independent player cameras.
- Player 1 uses WASD; Player 2 uses the arrow keys.
- No online multiplayer is included.

## ✨ Features

- **3D car and world rendering** powered by Three.js.
- **Garage customization** with five paint colours.
- **Interactive car preview**—drag to rotate the car in the menus.
- **Endless highway gameplay** with traffic and collision detection.
- **Two circuit tracks** with different layouts and difficulty ratings.
- **AI opponents** with different driving parameters.
- **Drifting and handbrake physics** in circuit races.
- **Three camera views** in circuit races.
- **Race HUD and minimap** showing position, lap, time, speed, and drift distance.
- **Procedural audio** using the Web Audio API, with a mute toggle.
- **Local browser saves** for the best Endless Traffic distance and Garage settings.
- **Responsive menus** and touch steering for Endless Traffic.

## 🖼️ Screenshots

### Garage & Customization

Choose one of five paint colours and set the Endless Traffic difficulty.

![OVERDRIVE Garage](assets/garage.png)

### 3D Car Preview

The menu preview can be rotated by dragging with a mouse or pointer.

![OVERDRIVE Car Preview](assets/car-preview.jpg)

## 🎯 Controls

### Endless Traffic

| Action | Keyboard |
|---|---|
| Steer left | `A` or `←` |
| Steer right | `D` or `→` |
| Boost / accelerate | `W` or `↑` |
| Brake | `S`, `↓`, or `Space` |
| Pause / resume | `Esc` or `P` |
| Mute / unmute | `M` |

**Touch:** Hold the left or right half of the screen to steer.

### AI Race

| Action | Keyboard |
|---|---|
| Accelerate | `W` or `↑` |
| Brake | `S` or `↓` |
| Steer | `A` / `D` or `←` / `→` |
| Handbrake / drift | `Space` or either `Shift` key |
| Change camera | `C` |
| Respawn | `R` |
| Pause / resume | `Esc` or `P` |

### Buddy Race

| Action | Player 1 | Player 2 |
|---|---|---|
| Accelerate | `W` | `↑` |
| Brake | `S` | `↓` |
| Steer left | `A` | `←` |
| Steer right | `D` | `→` |
| Handbrake / drift | `Left Shift` | `Right Shift` |
| Change camera | `C` | `/` |
| Respawn | `R` | `Enter` |

> Circuit racing is designed for keyboard input. Touch steering is available in Endless Traffic.

## 🏎️ Tracks & Race Settings

| Track | Difficulty |
|---|---|
| Sunset Circuit | Medium |
| Neon Hairpins | Hard |

- Race length: **1, 2, 3, or 5 laps**
- AI opponents: **1–5**
- AI difficulty: **Easy, Normal, or Hard**

## 🚀 Getting Started

OVERDRIVE is a single-page browser game. There is no build step or package installation.

1. Clone the repository:

   ```bash
   git clone https://github.com/testingElectroBAI/Overdrive.git
   ```

2. Open the project folder.

3. Run `index.html` in a modern browser, or start a local server:

   ```bash
   python -m http.server 8000
   ```

4. Open [http://localhost:8000](http://localhost:8000).

### Requirements

- A modern browser with WebGL support.
- An internet connection to load Three.js and Google Fonts from their CDNs.
- A keyboard for AI Race and Buddy Race.

## 🛠️ Built With

- **HTML5** — game structure.
- **CSS3** — interface, layout, and animations.
- **JavaScript** — gameplay, vehicle physics, AI, input, and state.
- **Three.js r128** — 3D rendering.
- **HTML Canvas** — procedural textures and track minimaps.
- **Web Audio API** — procedural audio.
- **Google Fonts** — Archivo Black and Space Mono.

## 📁 Project Structure

```text
Overdrive/
├── index.html
├── README.md
├── LICENSE
└── assets/
    ├── garage.jpg
    └── car-preview.jpg
```

The game, styles, and JavaScript are currently contained in the single `index.html` file. The `assets/` directory contains the README screenshots.

## 💾 Local Save Data

The game uses browser `localStorage`:

- `od_best` — best Endless Traffic distance.
- `od_cfg` — selected Garage paint colour and traffic difficulty.

This data stays in the current browser profile and is not synced to an account.

## ⚠️ Notes

- Buddy Race is local split-screen multiplayer, not online multiplayer.
- Track racing is keyboard-focused.
- Three.js and the selected fonts are loaded from external CDNs.
- Saved scores and Garage settings are browser-specific.

## 📄 License

This project is distributed under the [MIT License](LICENSE).

---

<div align="center">

### NO BRAKES. NO LIMITS. JUST DRIVE.

**OVERDRIVE © 2026**

</div>
