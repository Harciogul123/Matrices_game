# 🧩 Logic Puzzle Game (C++ / WinBGIm)

A logic puzzle game implemented in C++ using the `graphics.h` library. The objective is to fill an 8x8 grid by connecting colored dots or filling empty spaces, depending on the chosen game mode.

## 🎮 Game Modes

The application offers 3 distinct experiences:

1.  **Levels (Campaign):** 10 predefined levels with progressive difficulty.
2.  **Random:** Generates a random configuration of dots on the board for a unique challenge every time.
3.  **Custom:** Free mode where you can draw your own board layout.

## 🕹️ How to Play (Controls)

Interaction is done exclusively via mouse:

* **Left Click:**
    * Select menu options.
    * Draw path on the grid.
    * Place dots (in Custom mode).
* **Right Click:**
    * Activate color/dot to start drawing.
    * Change current color.
* **Menu Button:** Return to the main screen or reset current progress.

**Objective:** Completely fill the 8x8 matrix (`Board Full`) while respecting the color connection rules.

## 🛠️ Technical Requirements & Compilation

This project uses the **WinBGIm** library (a Windows port of the Borland BGI library). It will not run on a standard compiler without prior configuration.

### Requirements:
* **OS:** Windows.
* **IDE:** Code::Blocks (recommended) or MinGW with WinBGIm installed.
* **Compiler:** TDM-GCC (32-bit recommended).

### Important Configuration:
In the `main.cpp` file, the graphics initialization line is set to a specific path:
```cpp
initgraph(&gd, &gm, "C:\\TDM-GCC-32");
