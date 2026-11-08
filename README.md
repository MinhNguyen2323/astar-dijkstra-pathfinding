# A* & Dijkstra: Pathfinding Algorithms

**Graph Algorithms | Pathfinding | Python | Algorithm Visualization**

## 📌 Overview

This project explores two fundamental graph search algorithms, **Dijkstra's Algorithm and A* Search**, through Python implementations and interactive visualizations.

Two applications are developed:
- **Dijkstra:** Finding shortest paths in weighted, undirected graphs.
- **A*:** Planning routes for a multi-goal robotic vacuum cleaner under time-dependent cleaning costs.

The project focuses on algorithmic reasoning, object-oriented programming, search strategies, and practical trade-offs in pathfinding.

## 🔍 Methodology

### 1. Dijkstra's Algorithm

- Represent weighted graphs using nodes, edges, and adjacency structures.
- Implement shortest-path search with a priority queue (min-heap).
- Track minimum distances and reconstruct paths using predecessor information.
- Visualize graph exploration and shortest-path results.

**Core principle:** Repeatedly expand the node with the lowest known cumulative cost.

### 2. A* Search

- Model a robotic vacuum cleaner operating on a two-dimensional grid.
- Allow movement in eight directions and cleaning at multiple target locations.
- Apply Chebyshev distance as a heuristic for grid-based navigation.
- Use a greedy nearest-first strategy to select cleaning targets sequentially.
- Account for cleaning costs that increase as actions are performed.

**Core principle:** Combine accumulated path cost and estimated remaining distance to guide the search.

## 📊 Key Results

| Aspect | Dijkstra | A* |
|---|---|---|
| Application | Weighted graph navigation | Multi-goal robotic cleaning |
| Search Strategy | Uniform-cost expansion | Heuristic-guided search |
| Heuristic | Not required | Chebyshev distance |
| Output | Shortest path and total cost | Cleaning route and accumulated cost |
| Visualization | Graph exploration | Robot movement and cleaning actions |

**Experimental observations:**

- **Dijkstra:** Successfully demonstrated shortest-path computation and path reconstruction across four test scenarios.
- **A*:** Simulated robotic cleaning across three experimental scenarios, tracking movement, cleaning actions, and accumulated costs.
- **Key insight:** Heuristic guidance can prioritize promising search directions, while multi-goal planning introduces additional complexity because the order of visiting targets affects total cost.

## ⚖️ Strengths & Limitations

**Strengths**
- Object-oriented implementations with modular graph and environment structures.
- Visual demonstrations that make algorithm behavior easier to interpret.
- Practical applications of priority queues, graph traversal, and heuristic search.
- Exploration of pathfinding under both static edge weights and time-dependent cleaning costs.

**Limitations**
- Dijkstra requires non-negative edge weights and does not use heuristic guidance.
- A* performance depends on the heuristic and problem representation.
- The greedy nearest-first cleaning strategy does not guarantee a globally optimal multi-target cleaning plan.
- Larger search spaces may increase computational and memory requirements.

## 🛠️ Tech Stack

`Python` · `Jupyter Notebook` · `Object-Oriented Programming` · `Graph Algorithms` · `Priority Queues` · `Data Visualization`

## 📂 Repository Structure

```text
astar-dijkstra-pathfinding/
│
├── A-Star - Nhóm 06.ipynb
├── A-Star - Nhóm 06.docx
│
├── Dijkstra - Nhóm 06.ipynb
├── Dijkstra - Nhóm 06.docx
│
├── A-Star-and-Dijkstra-slides.pdf
└── README.md
```

## 📚 Academic Context

- **Course:** Data Analysis Programming
- **Institution:** University of Economics Ho Chi Minh City (UEH)
- **Project Type:** Collaborative academic coursework
- **Documentation:** Technical reports and presentation slides are included in the repository.

*This project demonstrates how algorithm design, heuristic selection, and problem constraints influence pathfinding behavior and computational efficiency.*
