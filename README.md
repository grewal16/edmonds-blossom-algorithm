# 🚀 Edmonds Blossom Algorithm

## Short Description
Dive deep into the fascinating world of graph theory with this robust C++ implementation of the renowned Edmonds Blossom Algorithm. Designed for efficiency and clarity, this project tackles the challenging problem of finding maximum matchings in general graphs, extending beyond the limitations of bipartite graphs. Whether you're a student, researcher, or competitive programmer, this repository offers a powerful tool and a comprehensive understanding of one of the most elegant solutions in algorithmic graph theory.

## ✨ Key Features
*   **Canonical Edmonds Blossom Implementation:** A highly optimized C++ realization of the celebrated algorithm for maximum matching.
*   **General Graph Support:** Solves the maximum matching problem on any type of graph, including those with odd cycles (blossoms).
*   **Exceptional Performance:** Leverages the power of C++ for rapid computation on complex graph structures.
*   **Visual Demonstrations:** Intuitive GIF animations (`Inputs.gif`, `Matching.gif`) showcasing graph inputs and the resulting maximum matching process.
*   **In-depth Documentation:** Accompanied by a detailed technical report (`Report_Implementation_of_Edmonds_Blossom_Algorithm.pdf`) providing a thorough analysis and explanation of the implementation.

## Who is this for?
*   **Computer Science Students:** Gaining practical experience with advanced graph algorithms and C++ development.
*   **Algorithm Enthusiasts:** Exploring the intricacies and implementation challenges of the Edmonds Blossom Algorithm.
*   **Researchers:** As a reference implementation or a foundational tool for further graph-theoretic studies and combinatorial optimization.
*   **Competitive Programmers:** A powerful and reliable resource for solving maximum matching problems in programming contests.

## Technology Stack & Architecture
*   **Core Language:** C++ (for high performance and low-level graph manipulation).
*   **Paradigm:** Procedural/Algorithmic.
*   **Focus:** Graph Theory, Data Structures, Combinatorial Optimization.
*   **Architecture:** A standalone, command-line executable application designed to process graph inputs and compute maximum matchings efficiently.

## 📊 Architecture & Database Schema
Given that this project implements a graph algorithm, a flowchart best illustrates the high-level execution flow and the core logic of the Edmonds Blossom algorithm.

```mermaid
graph TD
    A["`Start: Input General Graph G`"] --> B("`Initialize Empty Matching M`")
    B --> C{"`Can an augmenting path P be found from an unmatched vertex?`"}
    C -- "Yes" --> D("`Search for Augmenting Path P (using BFS/DFS)`")
    D --> E{"`Is an Odd Cycle ("#quot;Blossom"#quot;) detected during search?`"}
    E -- "Yes" --> F("`Contract Blossom into a Single Vertex`")
    F --> D
    E -- "No" --> G("`Augment Matching M along path P`")
    G --> C
    C -- "No" --> H("`End: M is a Maximum Matching`")
```

## ⚡ Quick Start Guide
To get this powerful algorithm running on your local machine, follow these simple steps:

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/grewal16/edmonds-blossom-algorithm.git
    cd edmonds-blossom-algorithm
    ```
2.  **Compile the Source Code:**
    Ensure you have a C++ compiler (like g++) installed on your system.
    ```bash
    g++ -std=c++11 -o graph graph.cpp
    ```
3.  **Run the Algorithm:**
    The compiled executable (`graph`) typically takes graph input from `stdin` or a file. For the expected input format, please refer to the `Inputs.gif` animation or the detailed `Report_Implementation_of_Edmonds_Blossom_Algorithm.pdf`.
    ```bash
    ./graph < input_graph.txt
    ```
    (Replace `input_graph.txt` with the path to your graph data file.)

## 📜 License
This project is open-sourced under the terms specified in the [LICENSE](LICENSE) file, detailing the conditions under which the software may be used, modified, and distributed.
