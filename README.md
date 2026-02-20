# 🚀 MySpaceInavder

> *A classic arcade-style space shooter game built with Python and Pygame*

[![Status](https://img.shields.io/badge/status-playable-success?style=flat-square)](.)
[![Python](https://img.shields.io/badge/python-3.x-blue?style=flat-square)](https://www.python.org/)
[![Pygame](https://img.shields.io/badge/pygame-2.x-green?style=flat-square)](https://www.pygame.org/)
[![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)](LICENSE)

---

## 📖 About

**MySpaceInavder** is a retro-style space shooter game where you defend Earth from incoming UFO invaders! Control your rocket ship, shoot down enemies, and try to reach the target score before missing too many ships.

🎮 **Classic Arcade Gameplay** — Simple controls, addictive action  
🎵 **Sound Effects & Music** — Immersive audio experience  
🏆 **Score System** — Track your progress and challenge yourself  
💥 **Fast-Paced Action** — Dodge and shoot your way to victory

---

## 🎯 Game Features

| Feature | Description |
|---|---|
| **Player Control** | Arrow keys to move left/right |
| **Shooting** | Spacebar to fire bullets |
| **Enemy Waves** | UFOs continuously spawn from the top |
| **Win Condition** | Destroy 10 UFOs to win |
| **Lose Condition** | Miss 3 UFOs (let them pass the bottom) |
| **Audio** | Background music + shooting sound effects |
| **Graphics** | Custom sprite assets (rocket, UFO, bullets) |

---

## 🚀 Getting Started

### Prerequisites
- Python 3.x
- Pygame library

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Momoiroart/MySpaceInavder.git
   cd MySpaceInavder
   ```

2. **Install Pygame:**
   ```bash
   pip install pygame
   ```

3. **Run the game:**
   ```bash
   python shooter_game.py
   ```

### Windows Executable
For Windows users, you can run the pre-built executable:
```bash
shooter_game.exe
```
No Python installation required!

---

## 🎮 How to Play

### Controls
- **←/→ Arrow Keys** — Move your rocket left/right
- **Spacebar** — Fire bullets
- **ESC** — Quit game

### Objective
- **Goal:** Shoot down 10 UFOs to win
- **Lives:** Don't let more than 3 UFOs escape past the bottom
- **Strategy:** Aim carefully and keep moving to avoid enemies

---

## 🗂️ Project Structure

```
MySpaceInavder/
│
├── shooter_game.py          ← Main game code
├── shooter_game.exe         ← Windows executable
├── shooter_game.spec        ← PyInstaller spec file
│
├── 📁 Assets (sprites & sounds)
│   ├── rocket.png           ← Player sprite
│   ├── ufo.png              ← Enemy sprite
│   ├── bullet.png           ← Bullet sprite
│   ├── asteroid.png         ← (Unused asset)
│   ├── galaxy.jpg           ← Background image
│   ├── space.ogg            ← Background music
│   └── fire.ogg             ← Shooting sound effect
│
├── LICENSE                  ← MIT License
└── README.md                ← You are here
```

---

## 🛠️ Tech Stack

| Component | Technology |
|---|---|
| Language | Python 3.x |
| Game Engine | Pygame |
| Graphics | PNG sprites |
| Audio | OGG sound files |
| Build Tool | PyInstaller (for .exe) |

---

## 🎨 Game Mechanics

### Sprite Classes

**GameSprite** — Base class for all game objects
- Position tracking (x, y)
- Speed control
- Image rendering

**Player** — Controllable rocket ship
- Arrow key movement
- Bullet firing
- Screen boundary collision

**Enemy** — UFO invaders
- Vertical movement
- Auto-respawn at top
- Miss counter on screen exit

**Bullet** — Projectiles
- Upward movement
- Auto-destroy at screen edge
- Collision detection

---

## 🏗️ Building the Executable

The `.exe` file was created using PyInstaller:

```bash
pyinstaller --onefile --windowed shooter_game.py
```

This bundles Python, Pygame, and all assets into a single executable.

---

## 🗺️ Development Roadmap

### ✅ Current Features
- [x] Player movement and shooting
- [x] Enemy spawning system
- [x] Collision detection
- [x] Win/lose conditions
- [x] Background music and SFX
- [x] Score tracking
- [x] Windows executable

### 🎯 Planned Improvements
- [ ] Power-ups (shields, rapid fire, etc.)
- [ ] Multiple enemy types
- [ ] Boss battles
- [ ] High score leaderboard
- [ ] Difficulty levels
- [ ] Asteroid obstacles
- [ ] Animation effects (explosions)
- [ ] Main menu and pause screen

---

## 🐛 Known Issues

- Typo in repository name ("Inavder" → should be "Invader")
- Asteroid sprite is unused in current version
- No pause functionality

---

## 🤝 Contributing

Want to add features or fix bugs? Contributions are welcome!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/NewPowerUp`)
3. Commit your changes (`git commit -m 'Add shield power-up'`)
4. Push to the branch (`git push origin feature/NewPowerUp`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- Built with [Pygame](https://www.pygame.org/)
- Inspired by classic Space Invaders arcade games
- Sound effects and sprites created/sourced for educational purposes

---

## 📊 Game Stats

- **Lines of Code:** ~200
- **Sprites:** 4 (rocket, UFO, bullet, background)
- **Sounds:** 2 (music + SFX)
- **Target Score:** 10 UFOs
- **Max Lives:** 3 misses

---

> **Play responsibly and aim true!** 🎯🚀✨
