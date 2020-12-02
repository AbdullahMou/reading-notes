[BACK](https://abdullahmou.github.io/reading-notes/)

# Linked Lists

![](https://files.realpython.com/media/Python-Linked-Lists-Guide_Watermarked.421631d9a615.jpg)

## What is a Linked List

* A Linked List is a sequence of Nodes that are connected/linked to each other
* the most defining feature of a Linked List is that each Node references the next Node in the link.

## Terminology

* Linked List - A data structure that contains nodes that links/points to the next node in the list.
* Singly - Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.
* Doubly - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.
* Node - Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.
* Next - Each node contains a property called Next. This property contains the reference to the next node.
* Head - The Head is a reference type of type Node to the first node in a linked list.
* Current - The Current reference is a reference type of type Node that is currently being looked at

## Traversal

* When traversing a linked list, you are not able to use a foreach or for loop.
* We depend on the Next value in each node to guide us where the next reference is pointing.
* The Next property is exceptionally important because it will lead us where the next node is and allow us to extract the data appropriately.

## Big O

* The Big O of time for Includes would be O(n).
* This is because, at its worse case, the node we are looking for will be the very last node in the linked list.
* n represents the number of nodes in the linked list.

## Adding a Node

* Adding O(1)

  *  If we want to add a node with an O(1) efficiency  
  * we have to replace the current Head of the linked list with the new node
  * without losing the reference to the next node in the list.

* Adding a Node O(n)

  * Adding a node to the middle of a linked list is a bit different than adding to the beginning.
  * This is because we are working with more nodes and must re-allocate to make room for the new node.

## Print Out Nodes

* Printing out all of the nodes in a Linked List is very similar to what we did in the` Find() `method.
* This is because we are leveraging our Current node and a while loop to traverse through the existing linked list.

## Prerequisites

* consider requiring a value to be passed in to require that each node has a value.
* When making a Linked List, you may want to require that at least one node gets passed in upon instantiation. This first node is what your Head and Current will point too.
