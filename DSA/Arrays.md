# Arrays

## What is an Array?

An array is a collection of elements stored in contiguous memory locations.

Example:

```python
arr = [10, 20, 30, 40, 50]
```

---

## Characteristics

- Same data type elements
- Contiguous memory allocation
- Fixed size in most languages
- Fast element access

---

## Operations on Arrays

### 1. Traversal

Visiting each element one by one.

Example:

```python
arr = [10,20,30]

for i in arr:
    print(i)
```

Time Complexity: O(n)

---

### 2. Accessing Element

```python
arr[2]
```

Time Complexity: O(1)

---

### 3. Insertion

Insert element at a specific position.

Time Complexity: O(n)

---

### 4. Deletion

Delete an element from an array.

Time Complexity: O(n)

---

### 5. Searching

#### Linear Search

Check each element one by one.

Time Complexity: O(n)

#### Binary Search

Works only on sorted arrays.

Time Complexity: O(log n)

---

## Time Complexity Table

| Operation | Complexity |
|------------|------------|
| Access | O(1) |
| Search | O(n) |
| Insertion | O(n) |
| Deletion | O(n) |

---

## Advantages

- Easy to use
- Fast access
- Efficient memory utilization

---

## Disadvantages

- Fixed size
- Insertion and deletion are costly

---

## Common Placement Questions

1. Two Sum
2. Maximum Subarray
3. Best Time To Buy And Sell Stock
4. Move Zeroes
5. Merge Sorted Array

---

## Interview Questions

Q1. Why is array access O(1)?

Answer:
Because memory addresses are contiguous and can be calculated directly.

Q2. Difference between Array and Linked List?

Array:
- Contiguous memory
- Fast access

Linked List:
- Dynamic size
- Easy insertion/deletion

---

## Revision Notes

- Access = O(1)
- Binary Search = O(log n)
- Traversal = O(n)
- Insertion/Deletion = O(n)
