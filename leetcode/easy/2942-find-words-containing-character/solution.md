# Find Words Containing Character

## Problem Information
- **Platform:** Leetcode
- **Difficulty:** Easy
- **URL:** https://leetcode.com/problems/find-words-containing-character/submissions/1905730204/
- **Date:** 2026-02-02

## Solution

```cpp
class Solution {
public:
    vector<int> findWordsContaining(vector<string>& words, char x) {
        vector<int> result;
        for (int i = 0; i < words.size(); ++i) {
            if (words[i].find(x) != string::npos) {
                result.push_back(i);
            }
        }
        return result;
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
