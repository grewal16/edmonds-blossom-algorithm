# 🚀 Edmonds Blossom Algorithm Implementation

## Short Description
Dive into the fascinating world of graph theory with this robust C++ implementation of the Edmonds Blossom Algorithm. This project provides a clear, efficient, and visually demonstrative solution for finding maximum cardinality matchings in general graphs, including those with odd cycles. It's a cornerstone algorithm for combinatorial optimization, brought to life with meticulous code and comprehensive documentation.

## ✨ Key Features
*   **Pioneering Algorithm:** A faithful and efficient implementation of Jack Edmonds' groundbreaking Blossom Algorithm for maximum cardinality matching.
*   **General Graph Support:** Capable of finding matchings in any graph, whether bipartite or non-bipartite, elegantly handling odd cycles through the "blossom contraction" technique.
*   **High-Performance C++:** Engineered in C++ for optimal speed and resource efficiency, making it suitable for competitive programming or academic research.
*   **Intuitive Visualizations:** Includes animated GIF examples (`Inputs.gif`, `Matching.gif`) that illustrate graph inputs and the computed maximum matching, providing invaluable insight into the algorithm's operation.
*   **In-Depth Documentation:** Accompanied by a detailed PDF report (`Report_Implementation_of_Edmonds_Blossom_Algorithm.pdf`) that thoroughly explains the theoretical foundations, implementation details, and analysis of the algorithm.

## Who is this for?
*   **Computer Science Students & Academics:** An excellent resource for learning and understanding advanced graph algorithms and combinatorial optimization.
*   **Algorithm Enthusiasts:** Anyone with a passion for algorithms and discrete mathematics looking to explore a classic problem and its elegant solution.
*   **Researchers:** A solid baseline implementation for further experimentation or integration into larger graph analysis projects.
*   **Competitive Programmers:** A powerful tool and learning aid for tackling complex graph matching problems in contests.

## Technology Stack & Architecture
*   **Primary Language:** C++ (demonstrated by `graph.cpp`)
*   **Core Algorithm:** Edmonds Blossom Algorithm
*   **Key Concepts:** Graph theory, maximum matching, augmenting paths, blossom contraction, adjacency lists/matrices (inferred for graph representation).

## 📊 Architecture & Database Schema
This project's architecture centers around the algorithmic flow of finding a maximum matching. Below is a high-level representation of the process, from input to the final result.

```mermaid
graph TD
    A[Graph Definition (Vertices & Edges)] --> B{Initialize Data Structures};
    B --> C{Search for Augmenting Path};
    C -- Path Found --> D[Blossom Contraction/Expansion & Path Augmentation];
    C -- No Path --> E[Maximum Matching Achieved];
    D --> C;
    E --> F[Output Max Matching & Size];

    style A fill:#e0f7fa,stroke:#00796b,stroke-width:2px;
    style F fill:#c8e6c9,stroke:#2e7d32,stroke-width:2px;
    style C fill:#fff3e0,stroke:#e65100,stroke-width:2px;
    style D fill:#ffe0b2,stroke:#ef6c00,stroke-width:2px;
```

## ⚡ Quick Start Guide
Get up and running with the Edmonds Blossom Algorithm in minutes!

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/grewal16/edmonds-blossom-algorithm.git
    cd edmonds-blossom-algorithm
    ```
2.  **Compile the Code:**
    Ensure you have a C++ compiler (like g++) installed.
    ```bash
    g++ -o graph graph.cpp -std=c++11
    ```
3.  **Run the Algorithm:**
    Execute the compiled program. The `graph.cpp` file is expected to handle graph input (likely hardcoded or via standard input) and output the matching.
    ```bash
    ./graph
    ```
    Observe the `Inputs.gif` and `Matching.gif` files in the repository for visual examples of typical inputs and the expected output matching. You may need to modify `graph.cpp` to experiment with different graph structures.

## 📜 License
This project is made available under an open-source license. For complete details regarding usage and distribution, please refer to the `LICENSE` file included in this repository.
