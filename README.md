# 🗺️ Route_X — Dijkstra Pathfinder Visualizer

A **Google Maps–style shortest path visualizer** built with pure HTML, CSS, and JavaScript. No frameworks, no libraries — just clean vanilla code that runs directly in your browser.

---

## 🚀 Live Demo

> Just download `index.html` and double-click it. That's it.

---

## 📸 Preview

| Step | What you see |
|------|-------------|
| Start selected | 🟢 Green node |
| Destination selected | 🔴 Red node |
| Algorithm running | 🟠 Orange flash (current) → 🟡 Yellow (visited) |
| Path found | 🔵 Blue trace (shortest path) |
| Blocked road | ⬛ Dark cell (obstacle) |

---

## ✨ Features

- **12 × 18 grid** of nodes representing a city map
- **Dijkstra's Algorithm** implemented from scratch with a Min-Heap priority queue
- **Step-by-step animation** — watch every node get explored in real time
- **Live distance updates** — each cell shows its current shortest distance as the algorithm runs
- **Obstacle mode** — block any road/intersection to create detours
- **Adjustable animation speed** — from slow-motion to fast-forward
- **Results panel** — shows nodes visited, path length, and total distance
- **Single file** — everything in one `index.html`, zero dependencies

---

## 🧠 How Dijkstra's Algorithm Works

1. Assign distance `∞` to all nodes, `0` to the start node
2. Push start into a **priority queue** (min-heap)
3. Always process the node with the **smallest known distance** first
4. For each neighbour, if a shorter path is found → update its distance and add to queue
5. Repeat until the destination is reached
6. **Backtrack** through `prev` pointers to reconstruct the shortest path

**Time Complexity:** `O((V + E) log V)` — V = nodes, E = edges

---

## 🎮 How to Use

```
1. Open index.html in any browser (double-click)
2. Click any grey node       → sets the START point (green)
3. Click another grey node   → sets the DESTINATION (red)
4. Click "Start Simulation"  → Dijkstra runs with animation
5. Click "Toggle Obstacle"   → then click nodes to block/unblock roads
6. Click "Reset"             → clears everything, new random weights
```

---

## 🛠️ Tech Stack

| Technology | Usage |
|------------|-------|
| HTML5      | Structure & grid layout |
| CSS3       | Animations, transitions, dark theme |
| JavaScript (ES6+) | Dijkstra's algorithm, Min-Heap, DOM manipulation |

> ⚡ Zero external libraries. Zero dependencies. Works offline.

---

## 📁 Project Structure

```
Route_X/
└── index.html      ← entire app (HTML + CSS + JS in one file)
```

---

## 🎨 Color Guide

| Color | Meaning |
|-------|---------|
| 🩶 Grey | Unvisited node |
| 🟢 Green | Start node |
| 🔴 Red | Destination node |
| 🟠 Orange | Currently processing |
| 🟡 Yellow | Visited / explored |
| 🔵 Blue | Final shortest path |
| ⬛ Black | Obstacle (blocked road) |

---

## 📌 Concepts Demonstrated

- Graph traversal with weighted edges
- Greedy algorithms (always pick minimum distance)
- Min-Heap / Priority Queue implementation
- Pathfinding and route reconstruction
- Async JavaScript for step-by-step animation
- CSS animations and transitions

---

## 👩‍💻 Author

**Suhani Sahu**  
📍 Built as a DSA + Frontend project  
🔗 [GitHub](https://github.com/suhanisahu)

---

## 📄 License

This project is open source and free to use for learning purposes.
