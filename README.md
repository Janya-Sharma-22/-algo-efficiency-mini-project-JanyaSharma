# -algo-efficiency-mini-project-JanyaSharma

My Project Overview

This project explores the time and space efficiency of fundamental algorithms.

The goal is to:
Implement algorithms in Python.
Experimentally measure time complexity and space usage using time and memory_profiler.
Visualize performance using matplotlib.
Document trade-offs, suitability, and stack/recursion depth risks.

Algorithms Implemented

Fibonacci-
Naïve Recursive
Dynamic Programming (Bottom-up)

Sorting Algorithms-
Merge Sort
Quick Sort
Insertion Sort
Bubble Sort
Selection Sort

Searching Algorithm-
Binary Search

| Algorithm             | Best Case  | Average Case | Worst Case |
| --------------------- | ---------- | ------------ | ---------- |
| Fibonacci (Recursive) | O(2^n)     | O(2^n)       | O(2^n)     |
| Fibonacci (DP)        | O(n)       | O(n)         | O(n)       |
| Merge Sort            | O(n log n) | O(n log n)   | O(n log n) |
| Quick Sort            | O(n log n) | O(n log n)   | O(n²)      |
| Insertion Sort        | O(n)       | O(n²)        | O(n²)      |
| Bubble Sort           | O(n)       | O(n²)        | O(n²)      |
| Selection Sort        | O(n²)      | O(n²)        | O(n²)      |
| Binary Search         | O(1)       | O(log n)     | O(log n)   |


Space Complexity Analysis

Fibonacci Recursive → O(n) (recursion stack).
Fibonacci DP → O(n), can be optimized to O(1).
Merge Sort → O(n) extra space.
Quick Sort → O(log n) recursion stack.
Insertion, Bubble, Selection → O(1) in-place.
Binary Search (iterative) → O(1), recursive → O(log n).
