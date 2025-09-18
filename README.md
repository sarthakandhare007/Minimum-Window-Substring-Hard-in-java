# Minimum-Window-Substring-Hard-in-java
🔹 Problem Statement

Given two strings s and t, return the minimum window substring of s such that every character in t (including duplicates) is included in the window.
If no such substring exists, return "".


---

🔹 Example

Input:  s = "ADOBECODEBANC", t = "ABC"
Output: "BANC"

Why?

"BANC" is the smallest substring of s that contains "A", "B", and "C".



---

🔹 Intuition (Sliding Window)

We use the sliding window technique with two pointers:

Expand the right pointer until the window contains all characters of t.

Then move the left pointer to shrink the window while it’s still valid.

Keep track of the smallest valid window seen so far.


We use a hashmap (or array) to store:

need: frequency of characters required from t

window: frequency of characters inside the current window of s

🔹 Complexity

Time: O(|s| + |t|) → each character is processed at most twice.

Space: O(|s| + |t|) → hashmap storage.



---

⚡ This is one of the most important sliding window problems — once you master it, you can solve:

Longest Substring Without Repeating Characters

Find All Anagrams in a String

Minimum Window Subsequence


