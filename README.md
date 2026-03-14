# ENPM661 Project 02 — Backward BFS & Backward Dijkstra Path Planning

Implementation of Backward BFS and Backward Dijkstra for a point robot navigating a custom obstacle map.

**Author:** Syed Yashal Ahmed (UID: 122288393)

---

## Overview

This repository is part of ENPM661 Project 02. It implements Backward BFS and Backward Dijkstra algorithms to find the optimal path for a point robot on a 180×50 mm map. The obstacle space is generated from the text "SYA 8393" with a 2 mm clearance around all obstacles and walls, and both algorithms animate node exploration and the final optimal path.

---

## Dependencies

* Python 3.9+
* pygame
* numpy
* scipy
* opencv-python

Install all dependencies with:

```
pip install pygame numpy scipy opencv-python
```

---

## Run Instructions

1. Clone the repository:

```
git clone https://github.com/username/ENPM661_Project02.git
cd ENPM661_Project02
```

2. Run Backward BFS:

```
python BW-BFS_firstname_lastname.py
```

3. Run Backward Dijkstra:

```
python BW-dijkstra_firstname_lastname.py
```

4. When prompted, enter the start and goal coordinates in mm (origin at bottom-left):

```
Enter START (x y) in mm, origin at bottom-left:  5 45
Enter GOAL  (x y) in mm, origin at bottom-left:  175 25
```

* Valid range: x in [0, 180),  y in [0, 50)
* If a coordinate falls inside an obstacle or clearance zone, you will be re-prompted

---

## Outputs

* **Pygame window** — 2-phase animation:
  * Phase 1: All explored nodes shown progressively in blue
  * Phase 2: Optimal path drawn in green
* **MP4 video file** saved automatically to the working directory:
  * `bfs_SYA8393.mp4`
  * `dijkstra_SYA8393.mp4`
* **Terminal output** — path length, total cost, nodes explored, and runtime

---

## Project Structure

```
ENPM661_Project02/
├── BW-BFS_firstname_lastname.py        # Backward BFS implementation
├── BW-dijkstra_firstname_lastname.py   # Backward Dijkstra implementation
├── bfs_SYA8393.mp4                     # BFS animation video (generated on run)
├── dijkstra_SYA8393.mp4                # Dijkstra animation video (generated on run)
└── README.md
```
