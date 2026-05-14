# 🧠 High Performance Rubik’s Cube Solver using Optimized Search Algorithms

## 📌 Overview
This project presents a high-performance Rubik’s Cube solver developed in Java, focusing on the comparative analysis of different state representations and search algorithms. The system explores how design choices in cube modeling and algorithm selection impact execution time, memory usage, and solution efficiency.

The project is implemented as part of a final-year BTech research initiative and aims to bridge theoretical concepts of algorithms with practical system performance.

---

## 👥 Team Members
- Ansh Oberoi (2210990138)  
- Ravneet Kaur (2210990720)

---

## 🎓 Supervisor
- Shikha Tuteja (Associate Professor, CSE Department)

---

## 📄 Project Type
- Research-Oriented Project  
- Research Paper submitted to ICDSA 2026 (Submission ID: 1737)

---

## 🎯 Objectives
- Design and implement multiple cube state representations  
- Apply and compare different search algorithms  
- Evaluate performance based on:
  - Execution time  
  - Memory usage  
  - Solution depth and efficiency  
- Identify optimal combinations of representation and solver  

---

## 🧩 Problem Statement
Efficiently solving the Rubik’s Cube involves navigating a massive combinatorial state space under strict computational constraints. This project investigates how different state representations and search strategies influence solver performance and scalability through systematic implementation and experimental evaluation.

---

## ⚙️ Features
- Multiple cube representation models  
- Implementation of classical and advanced search algorithms  
- Performance comparison framework  
- Command-line based execution  
- Modular and extensible architecture  

---

## 🧱 Cube Representations

### 1. 3D Array Representation
- Structure: 6 x 3 x 3 matrix  
- Stores each face explicitly  
- Simple to implement  
- High computational overhead during rotations  

### 2. 1D Array Representation
- Structure: Flattened 1 x 54 array  
- Better cache locality  
- Faster than 3D array  
- Requires index mapping logic  

### 3. Bitboard Representation
- Uses bit-level encoding for cube faces  
- Each face stored as a 64-bit structure  
- Highly memory efficient  
- Fast bitwise operations (rotations via shifts)  
- More complex implementation  

---

## 🔍 Solver Algorithms

### Breadth-First Search (BFS)
- Explores level by level  
- Finds shortest path  
- Very high memory usage  

### Depth-First Search (DFS)
- Explores deeply before backtracking  
- Low memory usage  
- Inefficient for deeper solutions  

### Iterative Deepening DFS (IDDFS)
- Combines advantages of BFS and DFS  
- Guarantees optimal solution  
- Controlled memory usage  

### Iterative Deepening A* (IDA*)
- Uses heuristic-based pruning  
- Highly efficient for deeper states  
- Best practical performance  
- Uses pattern database heuristics  

---

## 🧪 Performance Evaluation

The system evaluates different combinations of:
- Representation × Algorithm  

### Metrics:
- Execution Time  
- Memory Usage  
- Nodes Explored  
- Solution Depth  

### Goal:
Identify the most efficient configuration for solving the cube.

---

## 🏗️ System Design
- Object-Oriented Architecture  
- Modular design for:
  - Cube models  
  - Solver strategies  
- Easily extensible for adding new algorithms or heuristics  

---

## 🛠️ Technologies Used
- Java (Core Implementation)  
- Data Structures & Algorithms  
- JVM Memory Model  
- Git (Version Control)  

---

## 🚀 How to Run

### Prerequisites
- Java 8 or above  
- IntelliJ IDEA / VS Code / Terminal  

### Steps
git clone <repo-link>
cd rubiks-cube-solver
javac Main.java
java Main

---

## 📊 Experimental Setup
- Random cube shuffles are generated  
- Each solver runs on identical inputs  
- Results are recorded and compared across:
  - Different representations  
  - Different algorithms  

---

## 📈 Key Learnings
- Trade-offs between time and memory  
- Importance of efficient state representation  
- Limitations of brute-force approaches  
- Effectiveness of heuristic-based algorithms  
- Performance analysis and optimization  

---

## 🔮 Future Work
- Multi-threaded solver implementation  
- GPU acceleration  
- Advanced heuristics (corner-edge pattern database)  
- Web-based visualization  
- Real-time cube scanning integration  

---

## 📚 References
- Korf, R. E. – Optimal solutions using IDA*  
- Artificial Intelligence: A Modern Approach (Russell & Norvig)  
- Research papers on heuristic search and pattern databases  

---

## 📌 Submission Status
✔ Submitted to ICDSA 2026  
Submission ID: 1737  

---

## 📜 License
This project is intended for academic and research purposes.

---

## ⭐ Final Note
This project demonstrates how strong algorithmic design and system-level thinking can significantly impact performance, making it a solid foundation for both research and real-world applications.
