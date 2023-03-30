---
description: >-
  Usage: Monotonic Stack: Finding the next largest or smallest element in a
  list.
---

# Monotonic Queue and Monotonic Stack

Monotonic means the list or function is always increasing or decreasing. Before we push an element to it, we check if it breaks the condition. If it does we pop that element on the top till it satisfies the condition.

When using MS, we always store the index on to the stack rather than the value. This is because we can get the values from the list, but storing index gives us difference between the numbers.

A monostack stores **both the position and value**. The indices of the elements in the monostack are always increasing. The values of the elements are either monotonically increasing or decreasing.

The time complexity is O(n) for insert() and pop().&#x20;

### Monotonic Queue:

A variant of the above, if the next largest/smallest should be within the certain range or cerain distance or certain window, then use a **DEQUE,** so we can pop from the end of queue when the range exceeds.
