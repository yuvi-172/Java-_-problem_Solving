# Merge Intervals
## Problem Statement
Given a list of intervals, merge all overlapping intervals.

## Intuition
Sorting helps us process intervals in order, merging overlapping ones.

## Approach
1. *Sort intervals* by start time.
2. Use a *result list* to store merged intervals.
3. Iterate and merge overlapping intervals.
4. Return the merged intervals.

## Complexity Analysis
- *Time Complexity:* O(n log n) → Sorting dominates.
- *Space Complexity:* O(n) → Storing merged intervals.