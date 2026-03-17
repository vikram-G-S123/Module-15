# Ex. No: 15B - Build a Binary Search Tree Using Built-in Function

## AIM:
To write a Python program to build a binary search tree using a built-in function.

---

## ALGORITHM:

1. **Start the program.**
2. Define `_build_bst_from_sorted_values(sorted_values)` to recursively build a binary search tree (BST) from a sorted list.
3. Define `left_subtree(l)` to print the left subtree of the BST.
4. Take user input for the number of elements and store the values in a list `a`.
5. Sort the list and pass it to `_build_bst_from_sorted_values()` to construct the BST.
6. Print the postorder traversal of the BST.
7. Call `left_subtree(l)` to print the left subtree.
8. Check whether the tree is a binary search tree using the `is_bst` property.
9. **End the program.**

---

## PROGRAM:

```
# Name: Vikram GS
# Reg No: 212222060296

class Node:
    def __init__(self, value):
        self.value = value
        self.left = None
        self.right = None

root = Node(1.5)
root.left = Node(2.5)
root.right = Node(3.5)

print("Root:", root.value)
print("Left Child:", root.left.value)
print("Right Child:", root.right.value)


```

## OUTPUT
```
Root: 1.5
Left Child: 2.5
Right Child: 3.5

```

## RESULT

Binary tree with float values is created successfully.
