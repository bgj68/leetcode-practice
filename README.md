# LeetCode Practice

A collection of LeetCode solutions created to refresh and strengthen my computer science fundamentals, improve problem-solving skills, and prepare for technical interviews.

## Language
- Python

# 1. Two Sum

**Pattern:** Hash Map  
**Difficulty:** Easy  
**Concepts:** Arrays, Dictionaries, Time Complexity

## Approach

I used a hash map (Python dictionary) to store integers and their associated indices while iterating through the array. At each iteration, I calculated the complement by subtracting the current array element from the target value. If the complement had already been stored in the hash map, I returned the indices of the two numbers that summed to the target. Otherwise, I stored the current integer and its associated index for future lookup when it could become the complement of another array element.

## Key Takeaway

This problem demonstrated how hash maps can improve lookup efficiency. Instead of comparing every possible pair of numbers using a brute-force approach, I used previously stored values to find the solution in a single pass through the array.
