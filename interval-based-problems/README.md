# Interval Based problems

Introduction:

Interval questions are questions that give an array of two-element arrays (an interval). \
An example of an interval array: `[[1, 2], [4, 7]]`.

Question to ask : \
\- Clarify with the interviewer whether `[1, 2]` and `[2, 3]` are considered overlapping intervals, because it affects how you will write your equality checks.\
\- A common routine for interval questions is to sort the array of intervals by the start value of each interval.

```java
// Some code
Arrays.sort(intervals, (arr1,arr2)-> Integer.compare(arr1[0],arr2[0]));
```

\-Be familiar with writing code to check if two intervals overlap and to merge two overlapping intervals:

```
def is_overlap(a, b):  return a[0] < b[1] and b[0] < a[1]

def merge_overlapping_intervals(a, b):  return [min(a[0], b[0]), max(a[1], b[1])]


```

**Corner Cases:**&#x20;

* Single interval
* Non-overlapping intervals
* An interval totally consumed within another interval
* Duplicate intervals

\
