# 🚀 Edmonds Blossom Algorithm
<p align="center">
  <a href="https://github.com/grewal16/edmonds-blossom-algorithm/stargazers"><img src="https://img.shields.io/github/stars/grewal16/edmonds-blossom-algorithm?style=for-the-badge" alt="GitHub stars"></a>
  <a href="https://github.com/grewal16/edmonds-blossom-algorithm/network/members"><img src="https://img.shields.io/github/forks/grewal16/edmonds-blossom-algorithm?style=for-the-badge" alt="GitHub forks"></a>
  <a href="https://github.com/grewal16/edmonds-blossom-algorithm/issues"><img src="https://img.shields.io/github/issues/grewal16/edmonds-blossom-algorithm?style=for-the-badge" alt="GitHub issues"></a>
  <a href="./LICENSE"><img src="https://img.shields.io/github/license/grewal16/edmonds-blossom-algorithm?style=for-the-badge" alt="GitHub license"></a>
</p>

## Short Description
Dive deep into the fascinating world of graph theory with this robust C++ implementation of the Edmonds Blossom Algorithm. This project offers a clear, efficient, and well-documented solution for finding maximum cardinality matchings in general graphs, including those containing odd cycles (blossoms).

## 🛡️ Project Health & Status
This project provides a well-documented and functional implementation, ideal for academic study, research, and practical understanding of the Edmonds Blossom Algorithm. It is a stable, self-contained solution for graph matching problems.

## ✨ Key Features
*   **Complete Edmonds Blossom Algorithm:** A precise implementation of Jack Edmonds' groundbreaking algorithm.
*   **General Graph Support:** Handles arbitrary graphs, correctly identifying and contracting blossoms.
*   **Visual Demonstrations:** Includes GIF animations (`Inputs.gif`, `Matching.gif`) to visually illustrate algorithm execution and graph transformations.
*   **Comprehensive Documentation:** Accompanied by a detailed PDF report (`Report_Implementation_of_Edmonds_Blossom_Algorithm.pdf`) explaining the theoretical foundations and implementation specifics.
*   **C++ Efficiency:** Implemented in C++ for optimal performance and direct memory management.

## Who is this for?
This project is an invaluable resource for computer science students, researchers in graph theory and algorithms, competitive programmers, and anyone seeking a deeper understanding or a practical implementation of advanced graph matching techniques.

## Technology Stack & Architecture
This project is built using:
*   **Language:** C++

## 📊 Architecture & Database Schema
The project's architecture is focused on a singular, powerful algorithmic implementation:
*   The core logic for graph representation and the Edmonds Blossom Algorithm is encapsulated within `graph.cpp`.
*   Input graphs are processed directly by the algorithm to compute maximum cardinality matchings.
*   Interactive visualizations (via GIF files) highlight the algorithm's behavior on diverse graph structures.
*   Extensive theoretical and implementation insights are detailed in the included PDF report.

## ⚙️ Configuration & Deployment
This project is a standalone C++ application requiring no complex configuration. Simply compile the source code using a standard C++ compiler.

## ⚡ Quick Start Guide
To get started with this implementation:

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/grewal16/edmonds-blossom-algorithm.git
    cd edmonds-blossom-algorithm
    ```
2.  **Compile the Source Code:** Use a C++ compiler like `g++`.
    ```bash
    g++ graph.cpp -o graph
    ```
3.  **Run the Executable:**
    ```bash
    ./graph
    ```
    (Note: The program will likely expect graph input via `stdin` or has hardcoded examples. Refer to `graph.cpp` or the PDF report for specific input formats.)

## 📜 License
This project is licensed under the terms available in the `LICENSE` file.