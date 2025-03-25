```
def two_sum(nums, target):
    num_map = {}
    for index, num in enumerate(nums):
        complement = target - num
        if complement in num_map:
            return num_map[complement], index  # Returning indices
        num_map[num] = index
    return -1, -1  # Return -1, -1 if no valid pair is found

# Reading input in HackerRank format
n = int(input())  # Number of elements in the array
nums = list(map(int, input().split()))  # List of numbers
target = int(input())  # Target sum

# Solve and print result
index1, index2 = two_sum(nums, target)
print(index1, index2)
```
