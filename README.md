# -algo-efficiency-mini-project-JanyaSharma

My Project Overview

This project explores the time and space efficiency of fundamental algorithms.

The goal is to:
Implement algorithms in Python.
Experimentally measure time complexity and space usage using time and memory_profiler.
Visualize performance using matplotlib.
Document trade-offs, suitability, and stack/recursion depth risks.

INSTRUCTIONS:
1. Clone the Repository
 
[ git clone https://github.com/<your-username>/algo-efficiency-mini-project-<yourname>.git
cd algo-efficiency-mini-project-<yourname> ]

2. Install Dependencies
In Colab or local environment, install required packages:

[pip install matplotlib numpy memory_profiler jupyter]

3. Run Jupyter/Colab Notebook
Open notebook.ipynb in Google Colab or Jupyter.
Run each section to see profiling results and graphs.

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

#TRADE OFFS AND SUSTAINABILITY

Fibonacci (Recursive)

Suitability:
Easy to understand and implement.
Good for teaching recursion and basic algorithm analysis.
Trade-offs:
Very inefficient (O(2^n)) for large n.
Wastes computation by recalculating subproblems.
Not suitable for real-world applications beyond very small inputs.


Fibonacci (Dynamic Programming)

Suitability:
Much faster (O(n)) and efficient.
Good for large Fibonacci numbers.
Demonstrates the power of DP.
Trade-offs:
Uses extra memory (O(n)) for storing results.
Can be optimized further with "space-optimized DP" (only storing last 2 results).


Merge Sort

Suitability:
Efficient for large datasets (O(n log n)).
Stable sort (preserves order of equal elements).
Works well for linked lists.
Trade-offs:
Requires extra memory (O(n)), which can be costly for huge datasets.
Slower for small input sizes compared to simpler sorts.


Quick Sort

Suitability:
Fastest general-purpose sort in practice (O(n log n) average).
Works in-place, so low memory usage.
Trade-offs:
Worst case is O(n^2) (if pivots are bad).
Not stable.
Recursive implementation can cause stack overflow for huge arrays.


Insertion Sort

Suitability:
Great for small arrays.
Efficient when the array is almost sorted.
Very simple to implement.
Trade-offs:
O(n²) for large inputs.
Not good for big datasets.


Bubble Sort

Suitability:
Only for educational/demonstration purposes.
Helps beginners understand sorting concepts.
Trade-offs:
Extremely slow (O(n²)), never used in practice.
Inefficient even for moderately sized inputs.


Selection Sort

Suitability:
Simple to implement.
Good when memory writes are expensive (it does minimum swaps).
Trade-offs:
Still O(n²) → bad for large inputs.
Not stable by default.


Binary Search

Suitability:
Extremely efficient (O(log n)) for searching in sorted arrays/lists.
Great for databases, search engines, and real-time lookups.
Trade-offs:
Requires sorted data (if unsorted → need to sort first).
Not useful for dynamic data where inserts/deletes happen often.

Risks & Limitations:
+ Recursive algorithms may hit Python’s recursion depth limit (≈1000).
+ Memory profiling in Colab may show small fluctuations due to background processes.
+ Graphs represent empirical runtime, which can vary across machines.
