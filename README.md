# 🧠 LeetCode Solutions in C++

My personal collection of [LeetCode](https://leetcode.com/) solutions written in **C++**, while practicing data structures and algorithms. Each solution is named with the problem number and title so it's easy to find and revisit.

![Language](https://img.shields.io/badge/Language-C%2B%2B-00599C?logo=cplusplus&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-LeetCode-orange)
![Status](https://img.shields.io/badge/Status-Actively%20Updating-brightgreen)
[![LeetCode](https://img.shields.io/badge/LeetCode-Hepsiba__Selvi-FFA116?logo=leetcode&logoColor=white)](https://leetcode.com/u/Hepsiba_Selvi/)

## 📌 About

- Practicing problem solving to strengthen DSA fundamentals and interview preparation
- Solutions are written for clarity first, then optimized for time and space complexity
- Updated regularly as I solve more problems
- LeetCode profile: [Hepsiba_Selvi](https://leetcode.com/u/Hepsiba_Selvi/)

## 📂 Repository Structure

```
leetcode/
├── Easy/
│   └── 0001-two-sum.cpp
├── Medium/
│   └── 0003-longest-substring-without-repeating-characters.cpp
├── Hard/
│   └── ...
├── Database/        # MySQL problems
│   └── ...
├── Shell/           # Bash problems
│   └── ...
└── README.md
```

> Files are named `<problem-number>-<problem-name>.cpp` so they stay sorted.

## 📊 Progress

| Language | Problems Solved |
|----------|-----------------|
| C++      | 135             |
| MySQL    | 18              |
| Bash     | 2               |

🏅 **Badges:** 50 Days Badge 2026 · 100 Days Badge 2026

**Strongest topics:** Dynamic Programming, Divide and Conquer, Backtracking (advanced) · Math, Hash Table (intermediate) · Array, String, Two Pointers (fundamental)

> Stats are from my [LeetCode profile](https://leetcode.com/u/Hepsiba_Selvi/) and will be refreshed as I keep solving.

## 📝 Solutions Index

| # | Problem | Difficulty | Topic | Time | Space | Solution |
|---|---------|------------|-------|------|-------|----------|
| 1 | [Two Sum](https://leetcode.com/problems/two-sum/) | Easy | Array, Hash Table | O(n) | O(n) | [C++](Easy/0001-two-sum.cpp) |
|   |         |            |       |      |       |          |

## 🧩 Topics Covered

- Arrays & Strings
- Math
- Hash Tables
- Two Pointers & Sliding Window
- Linked Lists
- Stacks & Queues
- Trees & Graphs
- Recursion & Backtracking
- Dynamic Programming
- Divide and Conquer
- Sorting & Searching
- Greedy Algorithms
- SQL / Database queries (MySQL)

## 🚀 How to Run

LeetCode solutions are written as a `Solution` class, so to run one locally add a small `main()` that calls it.

```bash
# Clone the repository
git clone https://github.com/HepsibaMark/leetcode.git
cd leetcode

# Compile and run a solution
g++ -std=c++17 Easy/0001-two-sum.cpp -o solution
./solution
```

Example solution layout:

```cpp
#include <bits/stdc++.h>
using namespace std;

class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target) {
        unordered_map<int, int> seen;
        for (int i = 0; i < nums.size(); i++) {
            int need = target - nums[i];
            if (seen.count(need)) return {seen[need], i};
            seen[nums[i]] = i;
        }
        return {};
    }
};

int main() {
    Solution s;
    vector<int> nums = {2, 7, 11, 15};
    auto res = s.twoSum(nums, 9);
    cout << res[0] << " " << res[1] << endl;
    return 0;
}
```

## 🤝 Contributing / Feedback

This is a personal learning repo, but suggestions for cleaner or faster approaches are always welcome. Feel free to open an issue or pull request.

## 👩‍💻 Author

**Hepsiba Selvi M**
B.Tech AI & Data Science, Madras Institute of Technology, Anna University

- GitHub: [@HepsibaMark](https://github.com/HepsibaMark)
- LeetCode: [Hepsiba_Selvi](https://leetcode.com/u/Hepsiba_Selvi/)

---

⭐ If you find this useful, consider giving the repo a star!
