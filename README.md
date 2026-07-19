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

# 2. Valid Anagram

**Pattern:** Hash Map (Frequency Counting)
**Difficulty:** Easy  
**Concepts:** Dictionaries, Strings, Frequency Maps

## Approach

I first checked whether the two strings were the same length. If they were not, I immediately returned false because strings of different lengths cannot be anagrams. Next, I created two frequency maps using Python dictionaries. I iterated through each string separately and counted the number of occurrences of every character. I then compared the two dictionaries. If they contained the same characters with the same frequencies, the strings were anagrams. Otherwise, they were not.

## Key Takeaway

This problem reinforced the use of hash maps as frequency counters rather than lookup tables. Unlike Two Sum, where the dictionary stored a relationship between values and indices, this solution used dictionaries to track the number of times each character appeared. It also incorporated Python's .get() method for safely updating dictionary values.

# 3. Contains Duplicate

**Pattern:** Hash Set  
**Difficulty:** Easy  
**Concepts:** Arrays, Sets, Membership Checking

## Approach

I used a hash set to track values that had already appeared while iterating through the array. For each number, I first checked whether it already existed in the set. If it did, that meant it was a duplicate and I returned True. Otherwise, I added the number to the set and continued searching through. If the entire array was processed without finding a duplicate, I returned `False`.

## Key Takeaway

This problem reinforced the importance of choosing the correct data structure. Unlike previous problems where I needed to store additional information using a dictionary, this problem only required checking whether a value had been seen before. So, I used a set instead.
