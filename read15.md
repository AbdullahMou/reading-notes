
# Trees
* In this tutorial, we’ll be covering Binary Trees and Binary Search Trees. We will review some common terminology that is shared amongst all of the trees and then dive into specifics of the different types.

![](https://kevinvecmanis.io/assets/binary_trees/tree2.png)

## Common Terminology
**Node** - A node is the individual item/data that makes up the data structure

**Root** - The root is the first/top Node in the tree

**Left Child** - The node that is positioned to the left of a root or node

**Right Child** - The node that is positioned to the right of a root or node

**Edge** - The edge in a tree is the link between a parent and child node

**Leaf** - A leaf is a node that does not contain any children

**Height** - The height of a tree is determined by the number of edges from the root to the bottommost node

## Breadth First
* Breadth first traversal iterates through the tree by going through each level of the tree node-by-node. So, given our starting tree one more time:

* Traditionally, breadth first traversal uses a queue (instead of the call stack via recursion) to traverse the width/breadth of the tree. Let’s break down the process.

![](https://vivadifferences.com/wp-content/uploads/2019/10/DFS-VS-BFS.png)

## Binary Trees
* In all of our examples, we’ve been using a Binary Tree. Trees can have any number of children per node, but Binary Trees restrict the number of children to two 

## Binary Search Trees

* A Binary Search Tree (BST) is a type of tree that does have some structure attached to it.

* In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.

![](https://cdn.programiz.com/sites/tutorial2program/files/bst-vs-not-bst.png)

## Searching a BST

* Searching a BST can be done quickly, because all you do is compare the node you are searching for against the root of the tree or sub-tree. If the value is smaller, you only traverse the left side. If the value is larger, you only traverse the right side.

