# Trees Reading : 
### Trees : are data stuructures that has Binary Trees, Binary Search Trees, and K-ary Trees types.

## certain Common Terminology for trees :
* Node - A Tree node is a component which may contain its own values, and references to other nodes
* Root - The root is the node at the beginning of the tree
* K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
* Left - A reference to one child node, in a binary tree
* Right - A reference to the other child node, in a binary tree
* Edge - The edge in a tree is the link between a parent and child node
* Leaf - A leaf is a node that does not have any children
* Height - The height of a tree is the number of edges from the root to the furthest leaf

    **This figure below explains these terms :**
![](./BinaryTree1.png)



 * **how to traverse the tree ?**

Traversing a tree allows (to manipulate the tree) to search for a node, print out the contents of a tree, and much more! There are two categories of traversals when it comes to trees:


 **The ways to travers a tree :**
* Depth First
* Breadth First


### Depth First(stack) :

* Pre-order: root >> left >> right
* In-order: left >> root >> right
* Post-order: left >> right >> root

* **Pre-order: root >> left >> right** :

    Pre-order means that the root has to be looked at first. In our case, looking at the root just means that we output its value. When we call preOrder for the first time, the root will be added to the call stack:

    PreOrder 01

    Next, we start reading our preOrder function’s code from top to bottom. The first line of code reads this:

        OUTPUT <-- root.value (for the first root value) A

This means that we will output the root.value out to the console. Then, our next block of code instructs us to check if our root has a left node set. If the root does, we will then send the left node to our preOrder method recursively. This means that we make another function call, where B is our new root:
    OUTPUT <-- root.value (for the first root value) A,B

This process continues until we reach a leaf node. Here’s the state of our tree when we hit our first leaf, D:
    OUTPUT <-- root.value (for the first root value) A,B,D

It’s important to note a few things that are about to happen:

The program will look for both a root.left and a root.right. Both will return null, so it will end the execution of that method call
D will pop off of the call stack and the root will be reassigned back to B
This is the heart of recursion: when we complete a function call, we pop it off the stack and are able to continue execution through the previous function call.
The code block will now pick up where it left off when B was the root.

 Since it already looked for root.left, it will now look for root.right.



 E will output to the console. Since E is a leaf, it will complete the method code block, and pop E off of the call stack and make its way back up to B.
 In the function call, B has already checked for root.left, and root.right. There are no further lines of code to execute, so B will be popped off the call stack, so that we can resume execution of A.


        OUTPUT <-- root.value (for the first root value) A,B,D,E.

        
Following the same pattern as we did with the other nodes, A’s call stack frame will pick up where it left off, and check out root.right. C will be added to the call stack frame, and it will become the new function’s root.
C will be outputted to the console, and root.left will be evaluated. Because C has a left child, preOrder will be called, with the parameter root.left.
At this point, the program will find that F does not have any children and it will make its way back up the call stack up to C.

PreOrder 10

C does not have a root.right, so it will pop off the call stack and return to A.






        OUTPUT <-- root.value (for the first root value) A,B,D,E,C,F


### Breadth First(queue)
Breadth first traversal iterates through the tree by going through each level of the tree node-by-node. So, given our starting tree one more time:

Sample Tree

Our output using breadth first traversal is now:

        Output: A, B, C, D, E, F 





**Binary Tree Vs K-ary Trees**

In all of our examples, we’ve been using a Binary Tree. Trees can have any number of children per node, but Binary Trees restrict the number of children to two (hence our left and right children).

There is no specific sorting order for a binary tree. Nodes can be added into a binary tree wherever space allows. Here is what a binary tree looks like:
Binary Search Trees

**A Binary Search Tree** (BST)
 is a type of tree that does have some structure attached to it. In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.

**Big O**

The Big O time complexity of a Binary Search Tree’s insertion and search operations is O(h), or O(height). In the worst case, we will have to search all the way down to a leaf, which will require searching through as many nodes as the tree is tall. In a balanced (or “perfect”) tree, the height of the tree is log(n). In an unbalanced tree, the worst case height of the tree is n.

The Big O space complexity of a BST search would be O(1). During a search, we are not allocating any additional space.