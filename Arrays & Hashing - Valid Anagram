'''
Valid Anagram
Given two strings s and t, return true if the two strings are anagrams of each other, otherwise return false.

An anagram is a string that contains the exact same characters as another string, but the order of the characters can be different.

Example 1:
Input: s = "racecar", t = "carrace"
Output: true

Example 2:
Input: s = "jar", t = "jam"
Output: false
Constraints:

s and t consist of lowercase English letters.
'''

## Hash table
class Solution:
    def isAnagram(self, s: str, t: str) -> bool:
        s_res = {}
        t_res = {}
        if len(s) != len(t):
            return False

        for m in s:
            if m in s_res:
                s_res[m] += 1
            else:
                s_res[m] = 1
        
        for n in t:
            if n in t_res:
                t_res[n] += 1
            else:
                t_res[n] = 1

        for c in s_res:
            if s_res.get(c, 0) != t_res.get(c, 0):
                return False
        
        return True

## Sorting
class Solution:
    def isAnagram(self, s: str, t: str) -> bool:
        if len(s) != len(t):
            return False
        return sorted(s) == sorted(t)

## Hash Table
class Solution:
    def isAnagram(self, s: str, t: str) -> bool:
        if len(s) != len(t):
            return False

        s_res, t_res = {}, {}

        for i in range(len(s)):
            s_res[s[i]] = 1 + s_res.get(s[i], 0)
            t_res[t[i]] = 1 + t_res.get(t[i], 0)
        
        return s_res == t_res
