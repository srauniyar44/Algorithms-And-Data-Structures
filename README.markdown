# Assignment 3: Algorithm Efficiency and Scalability

## Overview
This repository contains the implementation and analysis for Assignment 3, focusing on Randomized Quicksort and Hash Table with Chaining. The code is written in Python, and the report details theoretical and empirical analyses.

## Repository Structure
- `assignment3.py`: Python implementation of Randomized Quicksort, Deterministic Quicksort, Hash Table with Chaining, and empirical testing scripts.
- `report.md`: Detailed report with theoretical analysis, empirical comparisons, and discussion.
- `README.md`: This file.

## Requirements
- Python 3.8+
- Libraries: `numpy`, `random`, `time`, `collections`

## How to Run
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```
2. Install dependencies:
   ```bash
   pip install numpy
   ```
3. Run the script:
   ```bash
   python assignment3.py
   ```
4. The script outputs sorting and hash table performance results for various input sizes and distributions.

## Summary of Findings
- **Randomized Quicksort**: Achieves \(O(n \log n)\) average-case time complexity, outperforming Deterministic Quicksort on sorted/reverse-sorted arrays due to random pivot selection.
- **Hash Table with Chaining**: Provides \(O(1)\) average-case insert, search, and delete operations, with performance maintained by dynamic resizing and universal hashing.
- Empirical results align with theoretical expectations, with minor overheads for small inputs or during hash table resizing.

## Notes
- The hash table uses a load factor threshold of 0.75 to trigger resizing.
- Sorting tests cover random, sorted, reverse-sorted, and repeated-element arrays.
- Results are printed to the console in a formatted manner.