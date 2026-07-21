# 🐺 Fenrir System — Tactical Activation Terminal

**Fenrir System** is an immersive web interface designed to activate mental and physical "protocols" for peak performance. Inspired by a tactical control terminal, it allows users to enter different flow states (sports, analytical, social) through step-by-step sequences, visual feedback, and a gamification system.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

---

## 📋 Table of Contents

- [Key Features](#key-features)
- [Available Protocols](#available-protocols)
- [Achievement System](#achievement-system)
- [Keyboard Shortcuts](#keyboard-shortcuts)
- [Data Persistence](#data-persistence)
- [Installation & Usage](#installation--usage)
- [Technologies Used](#technologies-used)
- [Screenshots](#screenshots)
- [Future Improvements](#future-improvements)

---

## ✨ Key Features

- **3 Tactical Protocols**: Each focused on a different performance area (sports, study, social leadership).
- **Immersive Activation Sequence**: Progress bar + real-time logs simulating system boot.
- **Dynamic ASCII Art**: The Fenrir mascot (wolf) changes appearance based on the active protocol.
- **Usage Statistics**: Activation counter and last use date for each protocol, automatically saved.
- **Achievement System (Gamification)**: 5 unlockable achievements with toast notifications and a dedicated modal.
- **Dark Terminal UI**: CRT aesthetics, micro-interactions, neon effects, and smooth animations.
- **Keyboard Shortcuts**: Quick navigation without using the mouse.
- **Full Persistence**: Data (stats, achievements, active protocol) stored in `localStorage` and `sessionStorage`.

---

## 🎯 Available Protocols

| Icon | Protocol       | Objective                         | Active Status |
|------|----------------|-----------------------------------|---------------|
| 🐺   | **Fenrir-Furia** | Sports domination (Football)      | WILD MODE     |
| 🧠   | **Fenrir-Mente** | Analytical precision (Exams)      | ANALYSIS MODE |
| 👑   | **Fenrir-Apex**  | Absolute presence and charisma    | ALPHA MODE    |

Each protocol contains a sequence of **4 tactical steps** that the user must follow to "activate" that mental/physical state.

---

## 🏆 Achievement System

The system monitors your activity and unlocks achievements automatically. When you earn one, a toast notification appears in the bottom-right corner and the badge counter updates.

| Achievement         | Icon | Unlock Condition                                      |
|---------------------|------|-------------------------------------------------------|
| **First Activation** | 🌟   | Activate any protocol for the first time.             |
| **Furia Master**     | 🐺   | Activate `Fenrir-Furia` a total of 5 times.           |
| **Mente Master**     | 🧠   | Activate `Fenrir-Mente` a total of 5 times.           |
| **Apex Master**      | 👑   | Activate `Fenrir-Apex` a total of 5 times.            |
| **Trifecta**         | 🔥   | Activate all 3 protocols on the same calendar day.    |

---

## ⌨️ Keyboard Shortcuts

| Key   | Action                                            |
|-------|---------------------------------------------------|
| `1`   | Activate the first protocol (**Fenrir-Furia**)    |
| `2`   | Activate the second protocol (**Fenrir-Mente**)   |
| `3`   | Activate the third protocol (**Fenrir-Apex**)     |
| `ESC` | Return to the main menu (closes views and modals) |

---

## 💾 Data Persistence

All user data is stored locally in the browser:

| `localStorage` key   | Content                                           |
|----------------------|---------------------------------------------------|
| `fenrir_stats`       | JSON object with counter and last use date of each protocol. |
| `fenrir_achievements`| JSON object with unlock status of each achievement. |
| `fenrir_last_protocol`| (Optional) Last used protocol.                   |

| `sessionStorage` key | Content                                           |
|----------------------|---------------------------------------------------|
| `fenrir_active`      | ID of the currently active protocol (to restore session on reload). |

---

## 🚀 Installation & Usage

This project is 100% frontend and requires no dependencies or servers.

1. **Clone the repository** (or download the `index.html` file):
   ```bash
   git clone https://github.com/your-username/fenrir-system.git
