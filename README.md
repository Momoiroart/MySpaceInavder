# MySpaceInvader

> Classic arcade-style space shooter built with Python and Pygame.

[![Python](https://img.shields.io/badge/python-3.x-blue?style=flat-square)](https://www.python.org/)
[![Pygame](https://img.shields.io/badge/pygame-2.x-green?style=flat-square)](https://www.pygame.org/)
[![GitHub](https://img.shields.io/badge/github-MySpaceInavder-7c4fd0?style=flat-square)](https://github.com/Momoiroart/MySpaceInavder)
[![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)](LICENSE)

---

## About

Defend Earth from UFO invaders! Control your rocket ship, shoot down enemies, and reach the target score before missing too many ships.

---

## Quick Start

### Requirements
- Python 3.x
- Pygame

```bash
git clone https://github.com/Momoiroart/MySpaceInavder.git
cd MySpaceInavder
pip install pygame
python shooter_game.py
```

### Windows (no Python needed)
```bash
shooter_game.exe
```

---

## Controls

| Key | Action |
|-----|--------|
| `←` / `→` | Move rocket left / right |
| `Spacebar` | Shoot |
| `ESC` | Quit |

---

## Rules

| Condition | Result |
|-----------|--------|
| Destroy 10 UFOs | **Win** |
| Miss 3 UFOs | **Lose** |

---

## Project Structure

```
MySpaceInavder/
│
├── shooter_game.py          ← Main game code (~200 lines)
├── shooter_game.exe         ← Windows executable (no install needed)
├── shooter_game.spec        ← PyInstaller build spec
│
├── rocket.png               ← Player sprite
├── ufo.png                  ← Enemy sprite
├── bullet.png               ← Bullet sprite
├── asteroid.png             ← Unused asset
├── galaxy.jpg               ← Background image
├── space.ogg                ← Background music
└── fire.ogg                 ← Shoot sound effect
```

---

## Tech Stack

| Component | Technology |
|-----------|------------|
| Language | Python 3.x |
| Engine | Pygame 2.x |
| Graphics | PNG sprites |
| Audio | OGG files |
| Build | PyInstaller |

---

## Game Mechanics

**Classes:**

| Class | Role |
|-------|------|
| `GameSprite` | Base: position, speed, render |
| `Player` | Arrow key movement, bullet firing, screen bounds |
| `Enemy` | Vertical fall, auto-respawn, miss counter |
| `Bullet` | Upward movement, collision detection, screen cleanup |

---

## Building the .exe

```bash
pip install pyinstaller
pyinstaller --onefile --windowed shooter_game.py
```

Output appears in `dist/`.

---

## Planned Features

- [ ] Power-ups (shields, rapid fire)
- [ ] Multiple enemy types
- [ ] Boss battles
- [ ] High score leaderboard
- [ ] Difficulty levels
- [ ] Main menu and pause screen
- [ ] Explosion animations

---

## Related Projects

| Project | Live | GitHub |
|---------|------|--------|
| **Portfolio** | [momoiro-workshop.vercel.app](https://momoiro-workshop.vercel.app/) | [momoiro-portfolio-dual](https://github.com/Momoiroart/momoiro-portfolio-dual) |
| **Learn Guide** | [learn-guide.vercel.app](https://learn-guide.vercel.app) | [conference-learn-guide](https://github.com/Momoiroart/conference-learn-guide) |

---

## Known Issues

- Repository name typo: "Inavder" instead of "Invader"
- `asteroid.png` is loaded but unused
- No pause functionality

---

## License

MIT — See [LICENSE](LICENSE) for details.
