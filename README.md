# LeetCode 297 - Serialize and Deserialize Binary Tree

## Problem Statement

Design an algorithm to serialize a binary tree into a string and deserialize the string back into the original binary tree.

The tree should be reconstructed with the same structure and values.

## Example

### Input

```text
root = [1,2,3,null,null,4,5]
```

### Output

```text
[1,2,3,null,null,4,5]
```

## Approach

Use preorder traversal.

For serialization:

* Visit the root.
* Visit the left subtree.
* Visit the right subtree.
* Store `null` when a node is missing.

For deserialization, read the values in the same order and rebuild the tree recursively.

## Algorithm

1. Start preorder traversal from the root.
2. Store each node value.
3. Store `null` for missing nodes.
4. Join all values into one string.
5. Split the string during deserialization.
6. Rebuild the tree recursively.

## Time Complexity

**O(n)**

## Space Complexity

**O(n)**

## Author

T. Nandhini
