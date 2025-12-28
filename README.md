# 🧨 Minesweeper in Power Apps (Canvas App)

This repository contains a **classic Minesweeper game** built as a **Power Apps Canvas App**, created to explore and showcase the **new Grid container** feature.

The project is intentionally small, nostalgic, and hands-on — focusing on layout, state management, and interaction patterns rather than business forms or CRUD scenarios.

---

## 🎯 Purpose

The main goals of this project were:

- to experiment with the **Grid container** in a realistic, grid-heavy scenario  
- to better understand **row/column–based layouts** in Canvas Apps  
- to test how far **Power Fx** can go for non-trivial interaction logic  
- and to have some fun rebuilding a classic many of us grew up with  

Minesweeper is a great candidate for this because it is:
- entirely grid-based  
- driven by clear spatial rules  
- fully state-dependent  
- instantly recognizable  

---

## 🧩 Features

- Classic **9 × 9 Minesweeper board** (Beginner-style)
- Random mine placement
- Adjacency calculation for surrounding mines
- Flood-fill behavior for empty cells
- Flagging mode with live mine counter
- Win / lose conditions
- Classic number coloring (1–8)
- Nostalgic UI inspired by the original Minesweeper
- Built entirely with **Power Fx**, no external services

---

## 🧱 Architecture & Design

### Grid container
The minefield is implemented using the **Power Apps Grid container**, using row and column semantics instead of absolute positioning. This makes the layout predictable, structured, and easy to reason about.

### State-driven design
All game state is stored in a single collection (`colCells`), which acts as the source of truth for:
- mine placement  
- revealed cells  
- flagged cells  
- adjacency counts  

UI elements react purely to state changes, keeping logic and presentation clearly separated.

### No external dependencies
The app runs entirely inside Power Apps:
- no connectors  
- no custom APIs  
- no Dataverse requirement  

---

## 🛠️ Technologies Used

- Power Apps (Canvas App)
- Power Fx
- Grid container
- Modern & classic Canvas controls

---

## 🚀 Getting Started

1. Clone or download this repository.
2. Import the Canvas App into your Power Apps environment.
3. Open the app in Power Apps Studio.
4. Run the app and start playing.

> **Note:** This project is intended as a learning and demo app, not a production game.

---

## 📸 Demo

A short demo video of the app in action is available on LinkedIn and can be added here as a GIF or MP4 if desired.

---

## 💡 Learnings

Some key takeaways from this project:

- The Grid container is a strong addition to Canvas Apps, especially for structured layouts.
- Thinking in rows and columns simplifies responsive design compared to absolute positioning.
- Power Fx scales surprisingly well when state is modeled cleanly.
- Rebuilding a familiar game is a great way to explore new platform features.

---

## 🙏 Inspiration

This project was inspired by a demo of the Grid container by **Reza Dorrani**, whose walkthrough helped spark the idea to try it out in a playful, hands-on way.

---

## ⚠️ Disclaimer

This project is not affiliated with Microsoft and is provided for educational purposes only.

---

## 📄 License

MIT License.
