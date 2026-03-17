# Ex. No: 15E - Build and Evaluate an Expression Tree

## AIM:
To write a Python program to build and evaluate the given Expression tree.

---

## ALGORITHM:

1. **Start the program.**
2. Create nodes for operators and operands.
3. Build the expression tree by connecting nodes in the correct hierarchical structure.
4. Define a recursive function `evaluate(root)`:
   - If the node is a number (leaf), return it.
   - Else, recursively evaluate left and right subtrees.
   - Apply the operator at the current node to the results.
5. Return the final result from the root node.
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

def evaluate(root):
    if root.left is None and root.right is None:
        return int(root.value)

    left_val = evaluate(root.left)
    right_val = evaluate(root.right)

    if root.value == '+':
        return left_val + right_val
    if root.value == '-':
        return left_val - right_val
    if root.value == '*':
        return left_val * right_val
    if root.value == '/':
        return left_val / right_val

# Expression: (3 + 2) * 4
root = Node('*')
root.left = Node('+')
root.right = Node('4')
root.left.left = Node('3')
root.left.right = Node('2')

print("Result:", evaluate(root))


```

## OUTPUT:
```
Result: 20

```

## RESULT:

Expression tree is built and evaluated successfully.

