"""
Valid Parentheses

Problem:
Given a string containing brackets, determine if the input
is valid based on matching pairs and ordering.

Approach:
Use a stack to store opening brackets.
When a closing bracket appears, compare it with the
most recent opening bracket.

Time Complexity: O(n)
Space Complexity: O(n)
"""


class Solution:
    def isValid(self, s: str) -> bool:
        pairs = {
            ")": "(",
            "]": "[",
            "}": "{"
        }

        stack = []

        for item in s:
            if item in "([{":
                stack.append(item)
            else:
                if not stack:
                    return False

                if stack[-1] == pairs[item]:
                    stack.pop()
                else:
                    return False

        return not stack
