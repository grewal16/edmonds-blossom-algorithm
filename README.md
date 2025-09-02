
# 🚀 Edmonds Blossom Algorithm Implementation

<p align="center"><img src="./Matching.gif" alt="Edmonds Blossom Algorithm in Action" width="700"></p>

## Short Description
Dive into the heart of graph theory with this robust C++ implementation of the **Edmonds Blossom Algorithm**! This project provides an efficient and clear solution for finding the maximum matching in any general graph, extending beyond the limitations of bipartite graphs. Whether you're a student, researcher, or simply fascinated by advanced algorithms, this repository offers a comprehensive resource, including a detailed report and visual demonstrations of the algorithm's powerful execution.

## ✨ Key Features
*   **Complete Edmonds Blossom Algorithm:** A fully functional C++ implementation to tackle maximum matching problems in general graphs.
*   **Visual Demonstrations:** Animated GIFs (`Inputs.gif`, `Matching.gif`) provide intuitive insights into graph construction and the matching process.
*   **Comprehensive Documentation:** A detailed PDF report (`Report_Implementation_of_Edmonds_Blossom_Algorithm.pdf`) explains the algorithm's theory, complexity, and implementation nuances.
*   **Modular C++ Codebase:** Clean and well-structured `graph.cpp` facilitating easy understanding, modification, and integration.
*   **Research & Educational Tool:** An ideal resource for learning, experimenting with, or building upon complex graph algorithms.

## Who is this for?
*   **Computer Science Students:** Gaining a deeper understanding of advanced graph algorithms and data structures.
*   **Researchers & Academics:** Exploring maximum matching problems, particularly in non-bipartite graphs.
*   **Algorithm Enthusiasts:** Those who enjoy dissecting and implementing complex, elegant solutions.
*   **Competitive Programmers:** Learning a powerful technique applicable to a wide range of graph challenges.

## Technology Stack & Architecture
This project is a pure, high-performance C++ implementation, focusing on algorithmic efficiency and clarity. It leverages standard C++ features and data structures to build a self-contained and effective solution without external dependencies or complex frameworks.

## 📊 Architecture & Database Schema
The core of this project is the **Edmonds Blossom Algorithm** itself, which iteratively refines a matching by finding augmenting paths. The process involves sophisticated graph traversal (BFS), cycle detection, and dynamic graph transformation (blossom shrinking and expansion). Here's a high-level overview of its operational flow:

```mermaid
graph TD
    A[Start Algorithm] --> B(Initialize Empty Matching M);
    B --> C{Find Augmenting Path P using BFS?};
    C -- "Yes" --> D{Odd Cycle ("Blossom") detected during BFS?};
    D -- "Yes" --> E[Shrink Blossom to Pseudo-Node];
    E --> C;
    D -- "No" --> F[Augment Matching M with P];
    F --> C;
    C -- "No" --> G(Return Maximum Matching M);
    G --> H[End Algorithm];
```

## ⚡ Quick Start Guide
To get this powerful algorithm up and running, follow these simple steps:

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/grewal16/edmonds-blossom-algorithm.git
    cd edmonds-blossom-algorithm
    ```
2.  **Compile the C++ Code:**
    Ensure you have a C++ compiler (like g++).
    ```bash
    g++ graph.cpp -o edmonds_blossom
    ```
3.  **Run the Executable:**
    The program will likely expect graph input. Refer to `Inputs.gif` or the `Report_Implementation_of_Edmonds_Blossom_Algorithm.pdf` for expected input formats.
    ```bash
    ./edmonds_blossom
    # ... then provide graph input as per the program's requirements
    ```

## 📜 License
This project is released under the **GNU General Public License v3.0**. See the `LICENSE` file for full details.
