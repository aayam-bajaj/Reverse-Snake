# 🍎🐍 Reverse Snake
### *You aren't the hunter. You're the snack.*

**Reverse Snake** is a high-octane, role-reversal arcade game. Instead of playing as a growing serpent, you control the **Food**. Your goal: survive a relentless, computer-controlled snake that grows larger and faster every second.

---

## 🚀 Live Demo
Play the game now in your browser:
### 👉 [https://reverse-snake-one.vercel.app/](https://reverse-snake-one.vercel.app/)

---

## 🕹️ The Concept
In the original Snake, the challenge was space management. In **Reverse Snake**, the challenge is **evasion**. 
The snake uses dynamic pathfinding AI to hunt you down. You must use your wits, the environment, and high-tech power-ups to avoid becoming a meal.

---

## ✨ Key Features

### 🌪️ Advanced Mechanics
* **Screen Wrapping:** The player can walk through walls to warp to the opposite side (Pac-Man style). Tricking the snake into a wall is a primary win condition!
* **Graze System:** Risk equals reward. Stay near the snake's head to build a **Graze Multiplier**, boosting your final Orb count by up to **4.0x**.
* **Teleportation:** Use the `T` key or tap the screen to instantly respawn at a random safe location.

### 💎 The Black Market
Spend **Orbs** earned during survival runs to buy permanent upgrades:
* **🔋 Hyper-Battery:** Increase maximum teleport capacity.
* **🧊 Cryo-Tech:** Extend the "Ice Cube" freeze duration.
* **🧪 Sluggish Serum:** Permanently slow the snake's base speed.
* **🍔 Food Skins:** Unlock the Burger, Pizza, or Neon Diamond skins.

### 🏆 Achievement System
Unlock unique achievements like **"Matador"** (tricking the snake into a crash) or **"Portal Jumper"** to claim massive Orb bounties.

---

## 🛠️ Technical Details

Reverse Snake is built with a focus on performance and "game feel," utilizing modern web standards to mimic a native application experience.

### 💻 Core Engine
* **HTML5 Canvas & ES6+:** The game rendering engine is built from scratch using the Canvas API for high-performance 2D drawing and a physics-based particle system.
* **AI Pathfinding:** The snake utilizes a customized distance-vector algorithm to calculate the shortest path to the player while avoiding its own body and managing "blind steps" during player teleports.
* **Responsive Scaling:** Implemented dynamic viewport scaling using CSS `min()` functions and Tailwind CSS to ensure a perfect 1:1 aspect ratio across all mobile and desktop resolutions.

### ☁️ Backend & Persistence
* **Firebase Firestore:** Real-time cloud synchronization for player save-states (`pData`).
* **Dual-Layer Storage:** A hybrid persistence model that utilizes **Firestore** for cross-device syncing and **LocalStorage** as a zero-latency fallback for offline play.
* **Firebase Auth:** Seamless anonymous authentication to track player history without requiring a tedious sign-up process.

### 🎹 Audio & UX
* **Web Audio API:** Features a procedural synthesizer that generates a **Dynamic Synthwave BGM**. The bassline frequency and tempo are tied directly to the `snakeSpeed` variable, creating a real-time auditory tension ramp.
* **Haptic Simulation:** Visual "Screen Shake" logic and CRT scanline filters provide tactile feedback for collisions and game events.

---

## 🎮 Controls
| Action | Keyboard | Mobile |
| :--- | :--- | :--- |
| **Move** | Arrow Keys / WASD | Precision Swipe |
| **Teleport** | `T` Key | Tap Screen |
| **Pause** | `P` / `Esc` | Auto-Pause on App Switch |

---
*Built with ❤️ for the retro gaming community.*
