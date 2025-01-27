
# 2D Spring Simulation

This project implements a **2D Spring Simulation** using SDL2. It visualizes the behavior of points connected by springs, with physics that includes gravity, spring forces, and damping. The user can interact with the simulation by adding/removing points and springs or applying forces dynamically.

---

## Getting Started

### Prerequisites
Ensure you have the following installed:
- C++ Compiler (e.g., g++)
*   [SDL2](https://www.libsdl.org/)
*   [SDL2_ttf](https://www.libsdl.org/projects/SDL_ttf/) (Not necessary)

## Project Structure

*   `sp.cc`: Main C++ source file.
*   `Makefile`: Build the project.
*   `src/`: Source code directory.
    *   `include/`: Header files.
    *   `lib/`: SDL related

### Installation
1. Clone the repository:
   ```bash
   git clone git@github.com:krishna23-45/Coding-a-Spring-Physics-Simulation.git
   ```
## Building

This project uses `make` for building. To build the project, run the following command in your terminal:

2. Navigate to the project directory:
   ```bash
   cd Coding-a-Spring-Physics-Simulation
   ```
3. Compile the code:
   ```bash
    make
   ```
4. Run the executable:
   ```bash
   ./spring_simulation
   
   ```
5. In window:
   ```bash
   main.exe
   ```
6. To clean up the build artifacts
   ```bash
    make clean
   ```
## Features

- **Physics-based simulation:**
    - Spring forces, damping, and gravity.
    - Collision with boundaries of the screen.
- **User interaction:**
    - Add points and connect them with springs using left mouse clicks.
    - Apply forces to points by right-clicking near them(points).
    - Remove the last added point and spring with the `R` key.
    - Fixed points can act as anchors in the simulation.
- **Visualization:**
    - Points are represented as small rectangles.
    - Springs are represented as lines connecting points.

---

---
## How to Use

1. **Start the simulation:**  
    Run the compiled binary to open a window with the simulation.

2. **Add points:**
    - Left-click anywhere in the window to add a point.
    - Each new point is connected to the previously added point with a spring.
3. **Apply forces:**
    - Right-click near points to push them away.
4. **Remove points:**
    - Press the `R` key to remove the last added point and its connecting spring.
5. **Exit the simulation:**
    - Press the `ESC` key or close the window.

---
## Key Controls

|**Action**|**Key/Mouse**|
|---|---|
|Add point and spring|Left mouse button|
|Apply force to points|Right mouse button|
|Remove last point/spring|`R` key|
|Exit simulation|`ESC` key|

---

## Code Overview

- **Core Physics:**
    - Spring forces are calculated based on Hooke's Law.
    - Damping reduces oscillations over time.
    - Gravity is applied to non-fixed points.
- **Structure:**
    - `Point` struct represents the position, velocity, and state of each point.
    - `Spring` struct connects two points and simulates spring dynamics.
    - Forces and collisions are recalculated every frame.
- **Rendering:**
    - Points are drawn as small rectangles.
    - Springs are drawn as lines between points.

---

---

## License

This project is licensed under the MIT License. Feel free to use, modify, and distribute the code.

---
## Acknowledgments

- SDL2 for graphics rendering.
- The concept of spring simulations from classical mechanics.
