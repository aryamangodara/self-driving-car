# 🚗 Self-Driving Car (No Libraries — Pure JavaScript)

[![Language](https://img.shields.io/badge/Language-JavaScript-F7DF1E?logo=javascript&logoColor=black)](#)
[![Libraries](https://img.shields.io/badge/Dependencies-None%20(Pure%20Vanilla%20JS)-green)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

A complete step-by-step implementation of a self-driving car simulation and neural network built from scratch using **pure JavaScript and HTML5 Canvas** — without external AI or physics libraries.

---

## 📌 Project Overview

This project explores autonomous driving mechanics, sensor simulation, collision detection, and neural network visualization. The car learns to navigate through traffic using evolutionary strategies and genetic algorithms (mutations) applied to a custom feed-forward neural network.

### ✨ Key Features
- **Zero External Dependencies**: Built entirely with Vanilla JavaScript and HTML5 Canvas API.
- **Physics & Mechanics**: Realistic acceleration, friction, turning radius, and boundary handling.
- **Ray-Casting Sensors**: Virtual distance sensors detecting road borders and simulated traffic obstacles.
- **Custom Neural Network**: Multi-layer perceptron implemented from mathematical principles.
- **Genetic Algorithm / Evolutionary Training**: Parallel car generation with mutation rate tuning and local storage persistence.
- **Real-Time Network Visualizer**: Interactive dynamic canvas displaying neuron activations and connection weights.

---

## 📂 Project Structure & Progression

The project is structured into progressive chapters demonstrating the incremental development of the system:

| Module | Topic | Description |
|---|---|---|
| **`1. Car driving mechanics`** | Basic Car Controls | Keyboard event handling, acceleration, friction, and steering physics. |
| **`2. Road definition`** | Environment & Borders | Infinite road rendering, lane computation, and border segments. |
| **`3. Artificial sensors`** | Ray Casting | Virtual lidar/radar rays casting from the car to detect intersections. |
| **`4. Collision detection`** | Polygon Intersections | Convex polygon collision tests between the car and road borders. |
| **`5. Traffic simulation`** | Dynamic Obstacles | Dummy traffic cars following lanes at varied speeds. |
| **`6. Neural network`** | Brain Architecture | Feedforward neural network evaluating sensor inputs to control steering. |
| **`7. Visualizing neural networks`** | Live Visualizer | Real-time visualization of weights, biases, and active layer signals. |
| **`8. Optimizing neural networks`** | Evolutionary Training | Running an ensemble of $N$ cars in parallel and picking the best performer. |
| **`9. Fine-tuning`** | Mutation & Storage | Saving best brain state to `localStorage` and mutating weights for progression. |
| **`10. Live stream variant`** | Advanced Experiments | Extended variants with additional tuning, track variations, and features. |

---

## 🚀 Getting Started

### Prerequisites
No Node.js or external package installation required. Any modern web browser (Chrome, Firefox, Edge, Safari) is supported.

### Running Locally
1. Clone or open this repository:
   ```bash
   git clone https://github.com/aryamangodara/self-driving-car.git
   cd self-driving-car
   ```
2. Open any module's `index.html` directly in your browser, or serve it using a local HTTP server:
   ```bash
   # Using Python 3
   python -m http.server 8000

   # Or using npx serve
   npx serve .
   ```
3. Navigate to `http://localhost:8000` and choose any chapter folder to view the simulation.

---

## 🎮 Controls & Interaction

- **Arrow Keys** (or **WASD**): Control the manual car (in early chapters).
- **Save Button (💾)**: Saves the current best-performing car brain to browser `localStorage`.
- **Discard Button (🗑️)**: Clears saved brain data to restart training from a fresh random state.

---

## 📚 References & Acknowledgments

- Based on the excellent YouTube tutorial series by [Radu Mariescu-Istodor](https://www.youtube.com/@radumariescu-istodor):
  - [Course Playlist Part 1](https://www.youtube.com/playlist?list=PLB0Tybl0UNfYoJE7ZwsBQoDIG4YN9ptyY)
  - [Course Playlist Part 2](https://www.youtube.com/playlist?list=PLB0Tybl0UNfZtY5IQl1aNwcoOPJNtnPEO)

---

## 📄 License

This repository is licensed under the [MIT License](LICENSE).
