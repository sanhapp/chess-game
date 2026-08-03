# ♟️ Chess Master — Cross-Platform Web Chess

A responsive, feature-rich HTML5 Chess game designed to run seamlessly across laptops, desktops, tablets, and mobile devices. Built using vanilla JavaScript, **Chess.js** for game logic, and **Chessboard.js** for interactive board rendering.

---

## ✨ Features

- 🎮 **4 Play Modes:**
  - **2 Player (Pass & Play):** Play locally with a friend on the same device.
  - **VS AI - Easy:** Random legal move AI, perfect for beginners.
  - **VS AI - Medium:** 2-ply depth positional evaluation AI.
  - **VS AI - Hard:** Minimax algorithm with Alpha-Beta pruning (3-ply depth search).
- 📱💻 **Dual Control Scheme (Cross-Platform):**
  - **Tap-to-Move (Mobile & Desktop):** Tap any piece (e.g., Knight/Horse) to highlight legal target squares, then tap your target square.
  - **Drag-and-Drop (Desktop):** Classic click-and-drag mouse controls.
- 💡 **Legal Move Highlight Guide:**
  - Selected piece highlights with a warm gold background.
  - All valid legal destination squares highlight with green indicator borders.
- ↩️ **Smart Undo System:**
  - Undoes 1 move in 2-Player mode.
  - Undoes 2 moves (Player + AI response) in VS AI modes.
- 👑 **Game State Recognition:**
  - Real-time turn tracking.
  - Automatic check, checkmate, stalemate, and draw notifications.
- 🎨 **Modern Dark Theme UI:** Sleek UI optimized for small mobile displays as well as high-resolution monitors.

---

## 🚀 Quick Start

No build tools or web servers are required!

1. Download or copy `index.html`.
2. Open `index.html` directly in any web browser (Google Chrome, Safari, Firefox, Microsoft Edge).
3. Select your desired game mode from the top dropdown and start playing!

---

## 🕹️ Controls Guide

| Input Method | Platform | How to Use |
| :--- | :--- | :--- |
| **Tap / Click** | Mobile & Laptop | Tap a piece to select it and show valid move guides. Tap a highlighted green square to move. Tap the piece again to deselect. |
| **Drag & Drop** | Laptop / PC | Click and drag any piece directly to an eligible target square. |

---

## 🛠️ Built With

- **HTML5 & CSS3** — Fully responsive layout with CSS variables and custom flex containers.
- **JavaScript (ES6)** — Core application logic and AI search implementation.
- **Chess.js** — Standard rules engine, move validation, check/checkmate detection, FEN parsing.
- **Chessboard.js** — Board UI widget and piece SVG rendering.
- **jQuery** — DOM manipulation and event binding.

---

## 🧠 AI Engine Details

The AI evaluates board positions based on piece values:
- **Pawn:** 10
- **Knight:** 30
- **Bishop:** 30
- **Rook:** 50
- **Queen:** 90
- **King:** 900

In **Hard Mode**, the computer employs a **Minimax Algorithm** enhanced with **Alpha-Beta Pruning** to search ahead 3 plies for optimal strategic moves without performance lag.
