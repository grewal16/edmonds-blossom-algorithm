# 🚀 Edmonds Blossom Algorithm Implementation

Dive deep into the fascinating world of graph theory with this robust C++ implementation of the **Edmonds Blossom Algorithm**! This project provides a precise and efficient solution to the critical challenge of finding maximum weight matchings in general graphs, a fundamental problem with wide-ranging applications from logistics to bioinformatics.

## Short Description

This repository presents a meticulously crafted C++ implementation of Jack Edmonds' groundbreaking Blossom Algorithm. It's designed to solve the problem of finding a maximum cardinality matching (or maximum weight matching with slight adaptation) in any arbitrary graph, extending beyond the simpler bipartite case. Explore a powerful algorithm made accessible, complete with clear code, visual demonstrations, and comprehensive documentation.

## ✨ Key Features

*   **Pioneering Algorithm:** A faithful and efficient C++ implementation of the Edmonds Blossom Algorithm.
*   **General Graph Support:** Solves maximum matching problems in any graph, including non-bipartite structures containing odd cycles (blossoms).
*   **Clear Visualizations:** Includes illustrative GIFs (`Inputs.gif`, `Matching.gif`) to demonstrate graph construction and the matching process.
*   **Comprehensive Documentation:** Accompanied by a detailed report (`Report_Implementation_of_Edmonds_Blossom_Algorithm.pdf`) explaining the algorithm's theory, implementation details, and analysis.
*   **Educational Resource:** An ideal resource for students, researchers, and developers exploring advanced graph algorithms.

## Who is this for?

*   **Computer Science Students:** Gaining a deeper understanding of advanced graph theory, matching algorithms, and C++ implementation practices.
*   **Algorithm Enthusiasts:** Exploring the elegance and complexity of one of the most significant algorithms in combinatorial optimization.
*   **Researchers & Academics:** A foundational reference or starting point for projects involving graph matching in various domains.
*   **Developers:** Those needing a clear, self-contained implementation of a maximum matching algorithm for general graphs.

## Technology Stack & Architecture

This project is built primarily with:

*   **C++:** The core algorithm logic and graph operations are implemented in C++.

The architecture revolves around the algorithm's procedural execution:
1.  **Graph Representation:** An efficient internal representation of the graph (likely adjacency lists or matrix).
2.  **Matching Logic:** The core Edmonds Blossom algorithm, involving BFS for augmenting paths, blossom detection, contraction, and expansion.
3.  **Input/Output:** Mechanisms to define graph inputs and present matching results.

## 📊 Architecture & Database Schema

The project implements a procedural algorithm rather than a database schema. Below is a simplified flowchart representing the core steps of the Edmonds Blossom Algorithm.

```mermaid
graph TD
    A[Start] --> B{Initialize Graph G & Empty Matching M};
    B --> C{Search for an Augmenting Path in G w.r.t. M?};
    C -- Yes --> D{Augment M along Path};
    C -- No --> E{Is an Odd Cycle (Blossom) Found?};
    E -- Yes --> F{Contract Blossom into a "Supernode"};
    F --> G{Recursively Search in Contracted Graph};
    G --> H{Expand Blossom & Adjust Matching};
    H --> B;
    D --> B;
    E -- No --> I[Return M (Maximum Matching)];
    I --> J[End];
```

## ⚡ Quick Start Guide

To get this powerful algorithm up and running on your local machine:

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/grewal16/edmonds-blossom-algorithm.git
    cd edmonds-blossom-algorithm
    ```

2.  **Compile the C++ Code:**
    Ensure you have a C++ compiler (like g++) installed.
    ```bash
    g++ -std=c++11 -O2 -Wall graph.cpp -o edmonds_blossom
    ```

3.  **Run the Executable:**
    Execute the compiled program. You may need to provide graph input as per the program's requirements (refer to `Report_Implementation_of_Edmonds_Blossom_Algorithm.pdf` for details on input format).
    ```bash
    ./edmonds_blossom
    ```
    Observe the output, which will detail the maximum matching found!

## 📜 License

A comprehensive `LICENSE` file is included in the repository root, outlining the terms and conditions for usage and distribution of this project. The specific license type is detailed within that file.
