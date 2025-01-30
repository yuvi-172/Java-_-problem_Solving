---

## 💡 Intuition
- A *sorted* array allows binary search.
- A *rotated sorted array* breaks the full order but maintains two sorted subarrays.
- The key idea is *determining which half is sorted* and *searching accordingly*.

---

## 🛠 Approach
1. *Use binary search* with two pointers: left and right.
2. **Find the middle element (mid).
3. **Check if mid is the target**, return its index.
4. *Determine which half is sorted*:
    - If nums[left] <= nums[mid], then the *left half is sorted*.
        - If target lies within this range, search in *left half*.
        - Otherwise, search in *right half*.
    - Otherwise, the *right half is sorted*.
        - If target lies within this range, search in *right half*.
        - Otherwise, search in *left half*.
5. Repeat until left > right.

---

## 📈 Complexity Analysis
| *Factor*     | *Analysis* |
|---------------|-------------|
| Time Complexity | *O(log n)* → Binary search reduces the search space by half each time. |
| Space Complexity | *O(1)* → No extra space is used. |

---