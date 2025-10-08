# 🚀 Edmonds Blossom Algorithm

## Short Description
Dive into the heart of graph theory with this robust C++ implementation of the Edmonds Blossom Algorithm! This project provides a clear, efficient, and well-documented solution for finding maximum matchings in **general graphs** – a fundamental problem in computer science and combinatorial optimization. Say goodbye to the limitations of bipartite graphs and unlock the power of matching in any graph structure.

## 🛡️ Project Health & Status
This project presents a stable and thoroughly documented academic implementation of the Edmonds Blossom algorithm, as evidenced by the comprehensive accompanying report. While designed for algorithmic clarity and correctness, it is ready for immediate use in research, educational settings, and as a foundation for advanced graph problems.

## ✨ Key Features
*   **Generalized Matching:** Accurately computes maximum matchings in *any* type of graph, including those with odd-length cycles (blossoms).
*   **Clear C++ Implementation:** Written in idiomatic C++ for performance and ease of understanding.
*   **Algorithmic Precision:** Implements the classic Edmonds Blossom algorithm with high fidelity.
*   **Visual Demonstrations:** Includes animated GIFs (`Inputs.gif`, `Matching.gif`) to visually illustrate the algorithm's operation and input/output.
*   **Comprehensive Documentation:** Supported by a detailed PDF report (`Report_Implementation_of_Edmonds_Blossom_Algorithm.pdf`) explaining the algorithm's theory and implementation specifics.

## Who is this for?
This project is an invaluable resource for:
*   Computer Science students and academics studying graph algorithms.
*   Researchers and practitioners in combinatorial optimization.
*   Competitive programmers seeking to understand and implement advanced matching algorithms.
*   Anyone curious about the elegant solution to the maximum matching problem in general graphs.

## Technology Stack & Architecture
This implementation is built predominantly using:
*   **Language:** C++
The core logic resides within a single, self-contained `graph.cpp` file, emphasizing a direct and efficient algorithmic approach.

## 📊 Architecture & Database Schema
The Edmonds Blossom Algorithm is an iterative process that refines a matching by finding augmenting paths and handling special structures called "blossoms."

```mermaid
graph TD
    A[Input Graph] --> B{Initialize Matching & Data Structures}
    B --> C{Search for Augmenting Path (BFS/DFS)}
    C -- No Path & Blossom Found --> D[Contract Blossom]
    D --> C
    C -- Augmenting Path Found --> E[Augment Matching & Expand Blossoms]
    E --> C
    C -- No Augmenting Path & No Blossom --> F[Maximum Matching Found]
```

## ⚙️ Configuration & Deployment
This project is a standalone C++ application. Configuration is minimal and involves standard C++ build practices. No complex environment setup, external services, or containerization are required.

## ⚡ Quick Start Guide
To get the Edmonds Blossom Algorithm up and running, simply follow these steps:

1.  **Clone the Repository (if applicable):**
    ```bash
    git clone https://github.com/grewal16/edmonds-blossom-algorithm.git
    cd edmonds-blossom-algorithm
    ```
2.  **Compile:** Use a standard C++ compiler (like g++) to compile the source file.
    ```bash
    g++ graph.cpp -o edmonds_blossom
    ```
3.  **Run:** Execute the compiled program. You will likely provide graph input via standard input or modify `graph.cpp` for specific test cases.
    ```bash
    ./edmonds_blossom
    ```
    (Refer to `Report_Implementation_of_Edmonds_Blossom_Algorithm.pdf` for specific input formats and usage examples.)

## 📜 License
This project is released under the **GNU General Public License v3.0**. See the `LICENSE` file for full details.