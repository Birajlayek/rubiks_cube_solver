# Algorithmic Rubik's Cube Solver

**Author**: Biraj Layek  
**Date**: May 2025  
**Project Status**: ✅ Completed  

---

## 1. Executive Summary

This report documents the development of a high-performance **Rubik's Cube (3x3) solver** in **C++**. The project focused on the practical application and performance analysis of both fundamental and advanced **graph traversal algorithms**. 

Three distinct class models were designed to represent the cube, allowing for a comparative study of data structure efficiency. The solver implements the following algorithms:

- **Breadth-First Search (BFS)**
- **Depth-First Search (DFS)**
- **Iterative Deepening DFS (IDDFS)**
- **Korf's Iterative Deepening A\* (IDA\*)**

The implementation achieved remarkable efficiency:
- **Moderately scrambled cubes (8 moves)**: Solved in under **3 seconds**
- **Complex configurations (13 moves)**: Solved in under **10 seconds**

---

## 2. Introduction & Project Objectives

The **Rubik's Cube** is a classic combinatorial puzzle that serves as an excellent case study for exploring **search algorithms** and **computational complexity**.

### Project Goals:

- 🧩 **Model the Rubik's Cube**  
  Design and implement an accurate and efficient C++ representation of a 3x3 cube.

- ⚙️ **Compare Data Structures**  
  Evaluate three different class models for cube representation to understand trade-offs in performance.

- 🔍 **Implement Search Algorithms**  
  Integrate multiple uninformed and informed search algorithms: BFS, DFS, IDDFS, and IDA\*.

- 🚀 **Achieve High Performance**  
  Solve scrambled cubes within tight time constraints.

- 📊 **Analyze Algorithmic Efficiency**  
  Empirically compare solving times of different algorithms on puzzles of varying complexity.

---

## 3. Technical Design and Algorithmic Implementation

The project was developed in **C++** to leverage its performance benefits and low-level memory control.

### Cube Representation

Three distinct C++ class models were created using:
- **Multi-dimensional arrays**
- **`std::vector` containers**

Each model was evaluated based on:
- Memory usage
- Manipulation ease (e.g., rotating faces)
- Overall algorithmic performance

### Search Algorithms Implemented

- 🔄 **Breadth-First Search (BFS)**  
  Guarantees the shortest path but is memory-intensive. Best for simple scrambles.

- 🧬 **Depth-First Search (DFS)**  
  Memory-efficient but does not guarantee optimal solutions.

- ⏳ **Iterative Deepening DFS (IDDFS)**  
  Combines DFS's memory efficiency with BFS's optimality via depth-limited iterations.

- 🧠 **Korf's IDA\* Algorithm**  
  An informed search using heuristics (e.g., pattern databases) to estimate steps to the goal. Efficient for deep scrambles.

---

## 4. Performance Results and Key Achievements

The solver was benchmarked against various scramble depths:

### 📊 Benchmark 1: Moderate Complexity
- **Scramble Depth**: 8 moves  
- **Algorithms Used**: BFS, DFS, IDDFS  
- **Result**: Solved in **< 3 seconds** consistently

✅ Demonstrates efficiency of cube modeling and basic search implementations.

---

### 📈 Benchmark 2: High Complexity
- **Scramble Depth**: 13 moves  
- **Algorithm Used**: Korf's IDA\*  
- **Result**: Solved in **< 10 seconds**

✅ Highlights the power of **heuristic-based search** in navigating vast state spaces where brute-force fails.

---

## 5. Conclusion

This project successfully transformed theoretical knowledge of computer science into a **practical, high-performance application**.

Key takeaways:
- ✅ Efficient cube modeling using C++
- ✅ Strategic use of multiple search algorithms
- ✅ Real-time solving of complex puzzles
- ✅ Strong emphasis on **performance** and **optimization**

The project showcases deep understanding in:
- Algorithm design
- Data structure efficiency
- Real-world problem-solving with C++

It stands as a testament to advanced **software engineering** and **AI search techniques**.

---

