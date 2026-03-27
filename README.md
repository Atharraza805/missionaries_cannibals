# ☠️ Missionaries & Cannibals

**A River-Crossing Puzzle of Logic & Survival**

A fully interactive, browser-based implementation of the classic **Missionaries and Cannibals** logic puzzle — featuring configurable group sizes, a BFS auto-solver, step hints, animated river crossing, and a complete state history table.

---

## 🎮 How to Play

The goal is to move **all missionaries and cannibals** from the **Left Bank** to the **Right Bank** using a boat — without ever letting cannibals outnumber missionaries on either side.

### Rules
- The boat can carry **1 to N people** per trip (configurable).
- At least **1 person** must be in the boat for each crossing.
- On **either bank**, if cannibals outnumber missionaries (and missionaries > 0), the missionaries get eaten — **game over**.
- Successfully move everyone to the Right Bank to **win**.

---

## ⚙️ Configuration

Before starting, you can customize:

| Setting | Range | Description |
|---|---|---|
| Missionaries | 1–5 | Number of missionaries to move |
| Cannibals | 1–5 | Number of cannibals to move |
| Boat Capacity | 2–4 | Max people per crossing |

Click **"Apply & Start New Game"** to begin with your settings.

---

## 🧩 Features

- 🔢 **Configurable puzzle** — adjust missionaries, cannibals, and boat capacity
- 🤖 **Auto-Solver** — BFS (Breadth-First Search) solves the puzzle instantly and animates the solution
- 💡 **Hint system** — reveals the next optimal move one step at a time
- 📋 **State History Table** — tracks every move with left/right bank counts, direction, and safety status
- ✅ **Safety validation** — real-time check prevents illegal moves
- 🎯 **Optimal step counter** — shows the minimum steps required for your configuration
- 🚤 **Animated boat** — visual river crossing with emoji characters
- 📖 **BFS Algorithm explained** — expandable section describing how the solver works

---

## 🧠 BFS Algorithm

The auto-solver uses **Breadth-First Search** to find the shortest valid path from the initial state `(M, C, LEFT)` to the goal state `(0, 0, RIGHT)`.

Each state is a tuple of `(left_missionaries, left_cannibals, boat_side)`. The solver explores all valid moves level by level, guaranteeing an **optimal solution** when one exists.

---

## 🚀 Getting Started

No build step required. Just open `index.html` in any modern browser.
```bash
git clone https://github.com/Atharraza805/missionaries-and-cannibals.git
cd missionaries-and-cannibals
open index.html
```

---

## 🛠️ Tech Stack

- **HTML5 / CSS3 / Vanilla JavaScript** — no frameworks, no dependencies
- BFS pathfinding implemented in pure JS
- CSS animations for boat and character movement

---

## 📸 Preview

> Setup screen with configurable missionaries, cannibals, and boat capacity — plus a live game board with move selector, event log, and state history.

---

## 📄 License

MIT License — free to use, modify, and distribute.
