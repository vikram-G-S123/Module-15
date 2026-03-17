# Ex. No: 15C - Expression Tree with Inorder and Postorder Traversal

## AIM:
To write a Python program to build the given expression tree and print the inorder and postorder traversals.

---

## ALGORITHM:

1. **Start the program.**
2. Import the required modules (`build` and `Node` from `binarytree`).
3. Define a list `x` representing the expression tree in pre-order fashion (with `None` for missing nodes).
4. Use the `build()` function to generate the binary tree.
5. Print the **inorder** and **postorder** traversal of the tree.
6. **End the program.**

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

def inorder(root):
    if root:
        inorder(root.left)
        print(root.value, end=" ")
        inorder(root.right)

def postorder(root):
    if root:
        postorder(root.left)
        postorder(root.right)
        print(root.value, end=" ")

# Sample Tree
root = Node('*')
root.left = Node('+')
root.right = Node('4')
root.left.left = Node('3')
root.left.right = Node('2')

print("Inorder Traversal:")
inorder(root)

print("\nPostorder Traversal:")
postorder(root)


```

## OUTPUT
```
Inorder Traversal:
3 + 2 * 4
Postorder Traversal:
3 2 + 4 *

```

## RESULT

Expression tree traversals are performed successfully.
