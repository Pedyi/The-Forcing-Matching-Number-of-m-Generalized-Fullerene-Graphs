# Forcing Matching Number of m-Generalized Fullerene Graphs

This repository contains the source code and computational algorithms used in the research paper:

> **"The Forcing Matching Number of m-Generalized Fullerene Graphs"** > *Authors: P. Asadzadeh, A. Behmaram, T. Došlić (2026)*

## Overview

The script `forcing_number_calculator.py` calculates the **Forcing Matching Number**, denoted as $f(G)$, for the family of m-generalized fullerene graphs $F(m,k)$.

The algorithm verifies the main theorem of the paper:
$$f(F(m,k)) = \lceil m/2 \rceil$$

### Key Features
* **Graph Generation:** Constructs the specific topology of $F(m,k)$ graphs using `networkx`.
* **Exact Computation:** Uses a backtracking algorithm with early termination to verify forcing sets.
* **Optimization:** Implements forced edge propagation (graph reduction) to handle larger instances.
* **Parallel Processing:** Utilizes Python's `multiprocessing` to efficiently analyze a wide range of parameters ($m$ and $k$).

## Usage

1.  **Dependencies:** Ensure you have Python installed along with the required libraries:
    ```bash
    pip install networkx numpy
    ```

2.  **Run the analysis:**
    ```bash
    python forcing_number_calculator.py
    ```

3.  **Output:** The results will be saved to `forcing_number_results.csv` with columns for `m`, `k`, and the computed forcing number.

## Citation

If you use this code in your research, please cite our paper:


