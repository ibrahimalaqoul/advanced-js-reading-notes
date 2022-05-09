# Hashtables :

concepts and  Terminology :
* Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.
* Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.
* Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

## Why do we use hash tables?
* Hold unique values
* Dictionary
* Library
## What Are they
Hashtables are a data structure that (used to store information) utilize  key value pairs.

The basic idea of a hashtable is the ability to store the key into this data structure, and quickly retrieve the value. This is done through what we call a hash. A hash is the ability to encode the key that will eventually map to a specific location in the data structure that we can look at directly to retrieve the value.
Hash table
From Wikipedia, the free encyclopedia
Jump to navigationJump to search
Not to be confused with Hash list or Hash tree.
"Rehash" redirects here. For the South Park episode, see Rehash (South Park). For the IRC command, see List of Internet Relay Chat commands § REHASH.
## Hash table
Type	Unordered associative array
Invented	1953
Time complexity in big O notation
Algorithm		Average	Worst case
Space		Θ(n)[1]	O(n)
Search		Θ(1)	O(n)
Insert		Θ(1)	O(n)
Delete		Θ(1)	O(n)

A small phone book as a hash table
In computing, a hash table, also known as hash map, is a data structure that implements a set abstract data type, a structure that can map keys to values. A hash table uses a hash function to compute an index, also called a hash code, into an array of buckets or slots, from which the desired value can be found. During lookup, the key is hashed and the resulting hash indicates where the corresponding value is stored.

Ideally, the hash function will assign each key to a unique bucket, but most hash table designs employ an imperfect hash function, which might cause hash collisions where the hash function generates the same index for more than one key. Such collisions are typically accommodated in some way.

In a well-dimensioned hash table, the average time complexity for each lookup is independent of the number of elements stored in the table. Many hash table designs also allow arbitrary insertions and deletions of key–value pairs, at amortized constant average cost per operation.[2][3][4]

Hashing is an example of a space-time tradeoff. If memory is infinite, the entire key can be used directly as an index to locate its value with a single memory access. On the other hand, if time is infinite, values can be stored without regard for their keys, and a binary search or linear search can be used to retrieve the element.[5]: 458 

In many situations, hash tables turn out to be on average more efficient than search trees or any other table lookup structure. For this reason, they are widely used in many kinds of computer software, particularly for associative arrays, database indexing, caches, and sets.