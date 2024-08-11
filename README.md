# Binary Tree Level Order Traversal

## Problem

Given root of binary tree, return level order traversal of its nodes’ values. (i.e., from left to right, level by level).

## Approach

Breadth-First Search (BFS) approach checks all nodes at present depth level before moving on to nodes at next depth level.

1. If root is None, return empty list.
2. Initialization beginning with root node in queue.
3. Loop until queue emptied
    - Get the number of nodes at current level.
    - Initialize empty list to store values of nodes at current level.
4. Iterate through all nodes at current level
    - Pop first node from queue.
    - Add its value to level list.
    - Add its children to queue if exist.
    - Add current level list to result list.
5. Return the list.

## Optimization

Time complexity of O(n), where n is number of nodes in tree, because each node checked once. Space complexity is also O(n) because of queue used for BFS.
