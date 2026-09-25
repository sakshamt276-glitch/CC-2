# CC-2-exp9 (24BDA70130)
## Problem Statement:78. Subsets
class Solution:
    
    def subsets(self, nums):
        result = []
        def backtrack(start, current):
            result.append(current[:])
            for i in range(start, len(nums)):
                current.append(nums[i])
                backtrack(i + 1, current)
                current.pop()
        backtrack(0, [])
        return result
