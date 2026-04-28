🧠 High Performance Rubik’s Cube Solver using Optimized Search Algorithms
📌 Overview

This project presents a high-performance Rubik’s Cube solver developed in Java, focusing on the comparative analysis of different state representations and search algorithms. The system explores how design choices in cube modeling and algorithm selection impact execution time, memory usage, and solution efficiency.

The project is implemented as part of a final-year BTech research initiative and aims to bridge theoretical concepts of algorithms with practical system performance.

👥 Team Members
Ansh Oberoi (2210990138)
Ravneet Kaur (2210990720)
🎓 Supervisor
Shikha Tuteja
📄 Project Type
Research-Oriented Project
Research Paper Submitted to ICDSA 2026 (Submission ID: 1737)
🎯 Objectives
To design and implement multiple cube state representations
To apply and compare different search algorithms
To evaluate performance based on:
Execution time
Memory usage
Solution depth and efficiency
To identify optimal combinations of representation + solver
🧩 Problem Statement

Efficiently solving the Rubik’s Cube involves navigating a massive combinatorial state space under strict computational constraints. The project investigates how different state representations and search strategies influence solver performance and scalability through systematic implementation and experimental evaluation.

⚙️ Features
Multiple cube representation models
Implementation of classical and advanced search algorithms
Performance comparison framework
Command-line based execution
Modular and extensible architecture
🧱 Cube Representations
1️⃣ 3D Array Representation
Structure: 6 x 3 x 3 matrix
Stores each face explicitly
✔ Simple to implement
❌ High computational overhead during rotations
2️⃣ 1D Array Representation
Structure: Flattened 1 x 54 array
✔ Better cache locality
✔ Faster than 3D array
❌ Requires index mapping logic
3️⃣ Bitboard Representation
Uses bit-level encoding for cube faces
Each face stored as a 64-bit structure
✔ Highly memory efficient
✔ Fast bitwise operations (rotations via shifts)
❌ Complex implementation
🔍 Solver Algorithms
🔹 Breadth-First Search (BFS)
Explores level by level
✔ Finds shortest path
❌ Very high memory usage
🔹 Depth-First Search (DFS)
Explores deeply before backtracking
✔ Low memory usage
❌ Inefficient for deeper solutions
🔹 Iterative Deepening DFS (IDDFS)
Combines BFS + DFS advantages
✔ Optimal solution guarantee
✔ Controlled memory usage
🔹 Iterative Deepening A* (IDA*)
Uses heuristic-based pruning
✔ Highly efficient for large depths
✔ Best practical performance
Uses pattern database heuristics
🧪 Performance Evaluation

The system evaluates different combinations of:

Representation × Algorithm
Metrics:
⏱ Execution Time
🧠 Memory Usage
🔄 Nodes Explored
📏 Solution Depth
Goal:

To determine the most efficient configuration for solving the cube.

🏗️ System Design
Object-Oriented Architecture
Modular design for:
Cube models
Solver strategies
Easy extensibility for adding:
New algorithms
New heuristics
🛠️ Technologies Used
Java (Core Implementation)
Data Structures & Algorithms
JVM Memory Model
Git (Version Control)
🚀 How to Run
Prerequisites
Java 8 or above
Any IDE (IntelliJ / VS Code) or terminal
Steps
# Clone repository
git clone <repo-link>

# Navigate to project
cd rubiks-cube-solver

# Compile
javac Main.java

# Run
java Main
📊 Experimental Setup
Random cube shuffles generated
Each solver tested on identical inputs
Results recorded and compared across:
Different representations
Different algorithms
📈 Key Learnings
Trade-offs between time and memory
Importance of efficient state representation
Practical limitations of brute-force search
Effectiveness of heuristic-based algorithms
Debugging concurrency and performance bottlenecks
🔮 Future Work
Multi-threaded solver implementation
GPU acceleration for search
Advanced heuristics (corner-edge pattern DB)
Web-based visualization interface
Integration with real-time cube scanning
📚 References
Korf, R. E. – Optimal solutions for Rubik’s Cube using IDA*
Artificial Intelligence: A Modern Approach (Russell & Norvig)
Research papers on pattern databases and heuristic search
📌 Submission Status

✔ Submitted to ICDSA 2026
Submission ID: 1737

📜 License

This project is intended for academic and research purposes.

⭐ Final Note

This project demonstrates how deep algorithmic understanding + system design can outperform surface-level implementations, making it a strong foundation for both research and real-world problem solving.
