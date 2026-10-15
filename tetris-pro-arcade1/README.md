# Tetris Pro Arcade 🕹️

> A tournament-grade, responsive Tetris arcade game built with React 19, TypeScript, Vite, and Tailwind CSS. Features Super Rotation System (SRS), Web Audio API chiptune synthesizer, 7-bag randomizer, multiple game modes, and customizable retro arcade themes.

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![React 19](https://img.shields.io/badge/React-19-61dafb.svg)
![TypeScript](https://img.shields.io/badge/TypeScript-5.0-3178c6.svg)
![Vite](https://img.shields.io/badge/Vite-6.0-646cff.svg)

---

## 🎮 Key Features

- **Standard Guideline Compliance**:
  - Full Super Rotation System (SRS) with wall kicks for all pieces (including complex I-piece kicks).
  - Authentic 7-Bag Randomizer (eliminates piece droughts).
  - Ghost Piece projection guide.
  - Hold Piece mechanism (with 1 swap lock).
  - Next Queue showing upcoming 4-5 pieces.
  - T-Spin detection (3-corner rule) with score bonuses.
  - Back-to-Back (B2B) Tetris and Combo streaks.

- **Game Modes**:
  - **Marathon**: Classic endless level progression with standard gravity ramp up to Level 20.
  - **Sprint (40 Lines)**: Race against the millisecond clock to clear 40 lines.
  - **Ultra (2-Minute Blitz)**: Score maximum points before the 120-second buzzer sounds.
  - **Zen / Practice**: Relaxed play with customizable gravity speed slider and infinite clears.

- **Pure Web Audio Synthesizer**:
  - Zero external MP3 or audio dependencies.
  - Real-time synthesized 8-bit sound effects (Move, Rotate, Hard Drop thud, Soft Drop, Hold chime, Tetris fanfare, Level-up, Game Over).
  - Authentic 8-bit chiptune background music (Korobeiniki / Tetris Theme A) with independent lead and bassline channels.

- **Arcade Themes**:
  - *Cyberpunk Neon* (Luminescent glow on ultra-dark glass)
  - *1989 Arcade* (Nostalgic Soviet arcade primaries)
  - *GameBoy 1989* (Authentic 4-shade greenish LCD dot-matrix)
  - *Midnight Minimal* (Clean contemporary graphite slate)
  - *Vaporwave Sunset* (Dreamy synthwave lilac & coral)

- **Input & Accessibility**:
  - Responsive keyboard controls with DAS (Delayed Auto Shift) & ARR (Auto Repeat Rate).
  - On-screen touch D-Pad and rotation controls for mobile & tablet gameplay.
  - High score persistence with `localStorage`.

---

## ⌨️ Controls

| Action | Primary Key | Secondary Key |
| :--- | :--- | :--- |
| **Move Left** | `ArrowLeft` | `A` |
| **Move Right** | `ArrowRight` | `D` |
| **Soft Drop** | `ArrowDown` | `S` |
| **Hard Drop** | `Space` | - |
| **Rotate Clockwise (CW)** | `ArrowUp` | `X` / `W` |
| **Rotate Counter-Clockwise (CCW)** | `Z` | `Left Ctrl` |
| **Hold Piece** | `C` | `Left Shift` |
| **Pause / Resume** | `P` | `Escape` |
| **Restart Game** | `R` | - |

---

## 🚀 Getting Started

### Prerequisites

- Node.js (version 18 or higher recommended)
- npm or pnpm

### Installation

```bash
# 1. Clone your repository
git clone https://github.com/<YOUR_GITHUB_USERNAME>/tetris-pro-arcade.git

# 2. Enter directory
cd tetris-pro-arcade

# 3. Install dependencies
npm install

# 4. Start local development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) (or the port Vite outputs) in your browser.

---

## 🌐 Deploy to GitHub Pages (Free)

1. In `vite.config.ts`, add your repo name as base:
   ```typescript
   export default defineConfig({
     base: '/tetris-pro-arcade/',
     // ...
   });
   ```
2. Build for production:
   ```bash
   npm run build
   ```
3. Push to a `gh-pages` branch or enable **GitHub Pages** from repository Settings -> Pages -> Source: GitHub Actions.

---

## 📄 License

This project is licensed under the MIT License - feel free to modify and share!

