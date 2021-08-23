# Reading 401-30: Hash Tables

## CodeFellows Docs: HashTables
This article is available [here](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html).

A has table is a data structure built to use an array to subdivide a data structure of key : value pairs for more efficient searching. This is accomplished via a hasing algorithm that converts a string key into an index in the array. A given key has a predictable hash value, which means that that index of the array can be referenced in order to find the key. 

We also need to define what happens when a second key lands at the same hash value. To handle this, we make the value of that index a LinkedList, and simply add nodes to the list to represent the additional pairs. 

## Paul Programming: What is a Hash Table?
This video is available [here](https://www.youtube.com/watch?v=MfhjkfocRR0).

This video gives a high level whiteboard demonstration of the structure of a hash table. The host draws out the structure and discusses some of the common uses of the structure. 

## HackerEarth: Basics of Hash Tables
This article is available [here](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/).

This article is yet another source that covers roughly the same ground on hash tables. Why were we given so many of these? 

Anyway, I will mention in this section that in order to read and add data to the table, we first convert to the hash, then traverse the linkedlist to add in a value (or find the one we are looking for). 

## Wikipedia: Hash Tables
This wikipedia entry is available [here](https://en.wikipedia.org/wiki/Hash_table).

This wiki offers more background information as well as a number of alternative hashing methods. It also discusses the time and space efficiency of various hash tactics, and the troubles of using them on small datasets. 

[<<Return to Home](../README.md)