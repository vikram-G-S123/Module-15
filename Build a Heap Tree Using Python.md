# Ex. No: 15D - Build a Heap Tree Using Python

## AIM:
To write a Python program to build a heap tree using appropriate Python package and function.

---

## ALGORITHM:

1. **Start the program.**
2. Import the `heapq` module.
3. Define a function `heaptree(H)` that takes a list `H` as input.
4. Use `heapq.heapify(H)` to convert the list into a min-heap.
5. Print the created heap.
6. **End the program.**

---

## PROGRAM:

```

# Name: Vikram GS
# Reg No: 212222060296

import heapq

heap = []

heapq.heappush(heap, 10)
heapq.heappush(heap, 5)
heapq.heappush(heap, 20)

print("Heap:", heap)

print("Smallest element:", heapq.heappop(heap))

```

## OUTPUT
```
Heap: [5, 10, 20]
Smallest element: 5

```

## RESULT
Heap tree is implemented successfully using heapq.
