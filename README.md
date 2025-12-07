# **Pac-Man A* Pathfinding — Google Colab Implementation**

This project is a fully animated **Pac-Man simulation** powered by **A* pathfinding**, dynamic ghost behavior, and automated video rendering. Designed for research, assignments, and visualization tasks, it showcases intelligent navigation inside a fixed **24×24 maze**, with real-time decision-making, food collection, ghost avoidance, and a polished GAME OVER / Completion sequence.

The system was implemented entirely in **Google Colab**, including rendering all frames and automatically exporting the final gameplay video.

---

## **📌 Key Features**

### 🔹 **A* Pathfinding for Smart Navigation**

* Pac-Man continuously re-plans optimal paths toward the nearest pellet.
* Dynamic cost adjustments discourage moving near ghosts.
* Predictive ghost positioning improves survival.

### 🔹 **Ghost Behavioral System**

* Two ghosts (B & C mix mode).
* Movement modes:

  * **Random / semi-random movement** before chase mode.
  * **Full chase algorithm** once Pac-Man eats a threshold number of pellets.
* Ghosts use A* pathfinding during chase.

### 🔹 **Full Visual Rendering (No Pygame Needed)**

* Rendered using **Pillow** (PIL).
* Emoji-style Pac-Man and Ghosts.
* Pixel-perfect grid maze.
* Real-time score, steps, and progress bar.

### 🔹 **GAME OVER and Completion Screens**

* Automatic overlay when Pac-Man is caught.
* Final "CONGRATULATIONS" screen when all pellets are collected.

### 🔹 **Video Output Generation**

* All animation frames stored in `/frames/`.
* Frames combined into `pacman_demo.mp4` automatically.
* Downloadable directly from Colab.

### 🔹 **Drive Backup Support**

* Script included to save:

  * Frames
  * Final video
  * Any generated files
    Directly into **Google Drive**.

---

## **📂 Project Structure**

```
Pac-Man-A*-Pathfinding/
│
├── pacman_main.ipynb       # Google Colab notebook
├── frames/                 # Output frames from simulation
├── pacman_demo.mp4         # Final game video
├── assets/                 # (Optional) Icons, fonts, extras
└── README.md               # Documentation
```

---

## **🚀 How to Run (Google Colab)**

1. Upload the notebook to Google Colab.
2. Run the dependency setup:

   ```bash
   pip install pillow imageio
   ```
3. Run the full script (A*, rendering, simulation).
4. Final video automatically appears for preview & download.
5. (Optional) Save results to Google Drive using:

   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```

   Folder name: **Pac-Man A* Pathfinding**

---

## **🎥 Output**

The project automatically produces:

* **High-resolution gameplay video**
* Smooth animation (8 FPS)
* Maze exploration
* Pac-Man’s A* path updates
* Ghost chase sequences
* Final GAME OVER or 100% Completion screen

---

## **📘 Use Cases**

* Pathfinding visualization
* Machine learning environment design
* Game AI demonstrations
* Academic assignments (DQN / RL integration)
* Research prototypes
* Maze-solving algorithm experiments

---

## **🧠 Concepts Demonstrated**

* A* Search
* Manhattan Heuristic
* Threat-aware cost penalties
* Multi-agent movement
* Predictive collision avoidance
* Grid-based rendering
* Animation pipelines
* File handling & video encoding

---

## **📜 Credits**

Developed in alignment with **Phase 3 workflow**, enhanced for clarity, visualization, and academic use.
Uses Python, Pillow, ImageIO, and Google Colab’s execution environment.

---

## **📄 License**

MIT License — free for personal, academic, and research use.

