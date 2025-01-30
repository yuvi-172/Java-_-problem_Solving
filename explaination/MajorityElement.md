# 🏆 Majority Element

## 📌 Problem Statement
Given an array nums of size n, return the *majority element*.  
The majority element is the element that appears *more than* ⌊n / 2⌋ times.  
You may assume that the majority element always exists in the array.

---

## 💡 Intuition
- The *majority element* appears *more than* n/2 times.
- If sorted, the **middle element (nums[n/2])** will always be the majority.
- We can solve this problem efficiently using *sorting, hash maps, or the Boyer-Moore Voting Algorithm*.

---

## 🛠 Approach 1: Sorting (Simple)
1. *Sort the array*.
2. The *middle element* nums[n/2] is guaranteed to be the majority element.
3. Return nums[n/2].

### 🔹 Complexity Analysis
| *Factor* | *Analysis* |
|------------|-------------|
| Time Complexity | *O(n log n)* → Due to sorting |
| Space Complexity | *O(1)* → No extra space used |

### ✅ Java Implementation
```java
package problems;
import java.util.Arrays;

public class MajorityElement {
    public static int majorityElementSort(int[] nums) {
        Arrays.sort(nums);
        return nums[nums.length / 2];  // Middle element is the majority
    }
}