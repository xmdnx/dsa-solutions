# Divisible and Non-divisible Sums Difference

## Problem Information
- **Platform:** Leetcode
- **Difficulty:** Easy
- **URL:** https://leetcode.com/problems/divisible-and-non-divisible-sums-difference/submissions/1905711286/
- **Date:** 2026-02-02

## Solution

```cpp
class Solution {
public:
    int differenceOfSums(int n, int m) {
        int sum_ndiv = 0;
        int sum_div = 0;
        for (int i=0; i<=n; ++i) {
            if (i % m) sum_ndiv += i;
            else sum_div += i;
        }
        return sum_ndiv - sum_div;
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
