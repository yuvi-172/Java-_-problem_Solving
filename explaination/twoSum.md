# *Two Sum (Leetcode - Medium)*
## 📝 Problem Statement
Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.

## 💡 Approach & Intuition
- Use a *HashMap* to store (value, index).
- For each number, check if target - nums[i] exists in the map.
- If found, return the indices; otherwise, store nums[i] in the map.

## ⏳ Time Complexity
- *O(n)* - We traverse the array once.

## ✅ Example
```java
Input: nums = [2, 7, 11, 15], target = 9
Output: [0, 1]