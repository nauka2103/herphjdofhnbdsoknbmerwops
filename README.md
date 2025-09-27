# Assignment 1: Divide-and-Conquer Algorithms

## 1. Implemented Algorithms
- **MergeSort**
    - Linear merge, reusable buffer, small-n cutoff.
- **QuickSort**
    - Randomized pivot, smaller-first recursion.
- **Deterministic Select (Median-of-Medians)**
    - Group of 5, recurse only into smaller side.
- **Closest Pair of Points**
    - Divide-and-conquer with strip optimization.

## 2. Architecture Notes
- Recursion depth bounded in QuickSort by tail recursion elimination.
- MergeSort uses a single reusable buffer.
- Select avoids recursion on unnecessary side.
- Closest Pair maintains sorted-by-y array for efficiency.

## 3. Recurrence Analysis
- **MergeSort**: T(n) = 2T(n/2) + Θ(n) → Θ(n log n) (Master, Case 2).
- **QuickSort**: T(n) = T(k) + T(n-k-1) + Θ(n).  
  Average: Θ(n log n). Worst: Θ(n²).
- **Select (MoM)**: T(n) = T(n/5) + T(7n/10) + Θ(n) → Θ(n).
- **Closest Pair**: T(n) = 2T(n/2) + Θ(n) → Θ(n log n).

## 4. Metrics & Plots
- Measured runtime vs input size.
- Recursion depth vs input size.
- Comparison of theory vs practice.
- Notes on constant-factor effects (cache, GC).

## 5. Testing
- Sorting tested on random and adversarial arrays.
- Select validated against Arrays.sort()[k].
- Closest Pair compared with O(n²) baseline for n ≤ 2000.

## 6. Summary
- Alignment between theoretical asymptotics and empirical measurements.
- QuickSort depth matches ~2 log2(n).
- Select consistently O(n).
- Closest Pair confirmed O(n log n).
# herphjdofhnbdsoknbmerwops
# test
# test
