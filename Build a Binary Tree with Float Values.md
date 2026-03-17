# Ex. No: 15A - Build a Binary Tree with Float Values

## AIM:
To write a Python program to build a binary tree with a root, left, and right node using floating-point values.

---

## ALGORITHM:

1. **Start the program.**
2. **Import** the `Node` class from the `binarytree` module.
3. **Create a root node** using the `Node` class and assign a floating-point value.
4. **Create left and right child nodes** for the root with float values.
5. **Convert the tree** to a list and print the list of nodes.
6. **End the program.**

---

## PYTHON PROGRAM

```
# Name: Vikram GS
# Reg No: 212222060296

import bisect

bst = []

elements = [10, 5, 15, 3, 7]

for el in elements:
    bisect.insort(bst, el)

print("BST (sorted list):", bst)
```

## OUTPUT
```
BST (sorted list): [3, 5, 7, 10, 15]

```

## RESULT

Binary Search Tree is simulated successfully using built-in functions.
