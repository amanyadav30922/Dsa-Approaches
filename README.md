# Dsa-Approaches

# Two Pointer Approach

The **Two Pointer Technique** is an efficient algorithmic approach mostly used in **Arrays**, **Strings**, and sometimes **Linked Lists**. It helps reduce time complexity from **O(n²)** to **O(n)** in many problems.

## Types of Two Pointers

### 1. Left-Right Pointer (Opposite Direction)

* `left` starts from the beginning.
* `right` starts from the end.
* Move pointers based on the condition.

### Logic

```cpp
if(sum < target)
    left++;

else if(sum > target)
    right--;
```

### When to Use

* Sorted Arrays
* Palindrome Problems
* Pair Sum Problems
* Optimization Problems

### Example

```cpp
Array = [2,7,11,15]
Target = 9

left = 0
right = 3

2 + 15 = 17 > 9
right--

2 + 11 = 13 > 9
right--

2 + 7 = 9
Answer Found
```

---

### 2. Fast-Slow Pointer (Same Direction)

* Both pointers start from the same side.
* One pointer moves faster than the other.

### Used In

* Linked List Cycle Detection
* Finding Middle of Linked List
* Removing Duplicates
* Sliding Window Problems

---

# Famous LeetCode Problems

## Easy

1. Two Sum II - Input Array Is Sorted (167)
2. Valid Palindrome (125)
3. Reverse String (344)
4. Remove Duplicates from Sorted Array (26)
5. Move Zeroes (283)
6. Squares of a Sorted Array (977)

## Medium

1. Container With Most Water (11)
2. 3Sum (15)
3. Sort Colors (75)
4. Reverse Words in a String (151)
5. String Compression (443)
6. Linked List Cycle II (142)

## Hard

1. Trapping Rain Water (42)
2. 4Sum (18)
3. Minimum Window Substring (76)

---

# Why Use Two Pointers?

### Brute Force

```cpp
O(n²)
```

### Two Pointer Approach

```cpp
O(n)
```

It eliminates unnecessary comparisons and provides an optimized solution for many interview problems.

## Key Idea

* If the array is sorted:

  * Sum is smaller than target → move `left++`
  * Sum is greater than target → move `right--`
  * Sum equals target → answer found

The Two Pointer Technique is one of the most important patterns for coding interviews and is commonly used in array and string problems. It is especially useful for pair-search, palindrome checking, sorted-array problems, and optimization tasks.
