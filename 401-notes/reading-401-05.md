# Reading 401-05: Linked Lists

## Code Fellows: Linked Lists
This article is available [here](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html).

A linked list is a classic data structure created by taking several node objects and linking them together in a chain. Each node genrally has a value and a next as properties, wherein the value contains the actual data we are interested in, and the next is a reference to the next node. This setup is repeated until each instance of node is tied together, forming a makeshift list. 

The list is generally managed and held together by an overarching class that keeps track of the Head (first node) and provides methods for interacting with the list. Because property keywords are not an effective way to navigate a linked list, these methods often traverse the list by keeping a reference to the "current" node in order to ground them, and then using each node's Next property to relocate to a later node in the chain, starting from the Head. 

## Vaidehi Joshi - What is a Linked List, Anyway? 
This article is in two parts, which can be found [here](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d) and [here](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996).

On one hand, a Linked List is similar to an array. The data is accessible through obedience to a specific order in a linear data structure. The primary difference, however, is that the linked list ia able to store its data more efficiently in memory by having each value located anywhere at all. Each node simply contains a refernce to the next, and that next could be anyplace, instead of in the same memory block as it must in an array value. 

Those references can have a couple of different variations, either with just a next in a straight lnie as alluded to above, or both a next and previous (doubly linked list) for traversing in either direction. In addition, the direction can leave the end node with a Next of NULL, or point it back to the head to form a circular linked list. 

A linked list also differs form an array in how it must be managed: Instead of adding to a sequence directly, we establish a new value and work on one of several options for rearranging the references. The important question is: "Where do I want this in my list? What does that mean about the new Node's pointers? Which node or nodes will need to point to the new one? from there we can appropriately change the refences to adjust to the new object with ease. 


[<<Return to Home](../README.md)