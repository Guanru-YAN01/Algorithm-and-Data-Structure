'''
Contains Duplicate
Given an integer array nums, return true if any value appears more than once in the array, otherwise return false.

Example 1:
Input: nums = [1, 2, 3, 3]
Output: true

Example 2:
Input: nums = [1, 2, 3, 4]
Output: false
'''

## Hash Set
class Solution:
    def hasDuplicate(self, nums: List[int]) -> bool:
        res = {}
        for num in nums:
            if num not in res:
                res[num] = 1
            else:
                res[num] += 1
                return True
        return False

## Hash Set Length
class Solution:
    def hasDuplicate(self, nums: List[int]) -> bool:
        return len(set(nums)) < len(nums)

## Sorting
class Solution:
    def hasDuplicate(self, nums: List[int]) -> bool:
    nums.sort()
    for i in range(1, len(nums)):
        if nums[i] == nums[i-1]:
            return True
    return False

