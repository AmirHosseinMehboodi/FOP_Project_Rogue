# 🗡️ Terminal-Based Roguelike RPG 🛡️

## 📜 Description
A classic, terminal-based Roguelike dungeon crawler written entirely in C using the `ncurses` library. Developed as the Phase 1 project for the Fundamentals of Programming course at Sharif University of Technology, this game features procedural map generation, resource management, and a file-based user authentication system. 

It was designed to run directly in the terminal, utilizing ASCII/Unicode graphics to render dynamic environments, items, and menus.

## ✨ Key Features
* **🔐 User Authentication System:** Includes a fully functional sign-up and login menu. Validates username availability, enforces strong password constraints, checks email formatting, and persistently stores user data via file I/O.
* **🏰 Procedural Dungeon Generation:** Dynamically generates randomized, non-overlapping rooms and connects them with corridors. Dungeons feature varying themes, hidden doors, pillars, and distinct start/exit points.
* **🎒 Inventory & Resource Management:** Players must manage hunger and health by looting different types of food, weapons (swords, daggers, wands), and magical potions (health, speed, strength).
* **👁️ Dynamic Rendering:** Utilizes `ncurses` for terminal manipulation, handling color pairings, keyboard interrupts (arrow keys/vim keys for 8-way movement), and line-of-sight map exploration (fog of war).
* **💾 Game State Persistence:** Built with the architecture to save and load player progress and explored maps across sessions.

## 🛠️ Tech Stack
* **Language:** 💻 C
* **Libraries:** 📚 `<ncurses.h>`, `<stdlib.h>`, `<unistd.h>`

## 🚀 How to Run

1. Make sure you have the `ncurses` library installed on your system (e.g., `sudo apt-get install libncurses5-dev libncursesw5-dev` for Debian/Ubuntu).
2. Clone the repository.
3. Compile the code using GCC:
   ```bash
   gcc 0.1.6.c -lncurses -o rogue_game
