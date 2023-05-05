Download Link: https://assignmentchef.com/product/solved-cse222-homework-4
<br>
<strong><u>PART 1:</u></strong>

You should implement the following features for the Heap structure.




<ol>

 <li>Search for an element</li>

 <li>Merge with another heap</li>

</ol>

<ul>

 <li>Removing i<sup>th</sup> largest element from the Heap</li>

</ul>

<ol>

 <li>Extend the Iterator class by adding a method to set the value (value passed as parameter) of the last element returned by the next methods.</li>

</ol>




<strong><u>PART 2: </u></strong>

You should implement a BSTHeapTree class that keeps the elements in a Binary Search Tree where the nodes store max-Heap with a maximum depth of 2 (maximum number of elements included in a node is 7).

An example of this class is below.




When implementing the class, you must adhere to the following features:

<ol>

 <li>Each node in the heap holds two data: a value (an integer in the example above) and the number of occurrences of the value (how many that number is added to the tree). In the example, the notation 37.1 means that the number 37 is there is only one occurrence of the value 37 is available in the container.</li>

 <li>Movement on BST is based on values at the root nodes of the Heap. In the example, the root nodes of Heaps are shown in red. If you want to add the number 50 to the tree, the movement will be done as follows:</li>

</ol>

Since the Heap with root 37 is full, since 50 is not an element of this Heap and  50 &gt; 37, it moves to the right node in BST.

Since the Heap with root 124 is full, since 50 is not the element of this Heap and 50 &lt; 124, it moves to the left node in BST.

Since the Heap with root 60 does not have the number 50 and there is space, it is inserted into the heap at this node as (50.1).

<ol start="3">

 <li>If the Heap at a node of BST is full and a new number still needs to be added, a new BST node should be created as the left or the right child of the BST node. After the Heap in the root node of the BST in the example is filled, when a number smaller than 37 is inserted, the left child is created, and the number is inserted into the new Heap in that node. When we examine the example, there are 7 numbers smaller than 37 are inserted into the left child (one 31, one 15, one 29 and four 13’s).</li>

 <li>Remove operation removes only one occurrence of the value. If the number of occurrences becomes zero than the value should be removed.</li>

 <li>During a remove operation, if the heap at a node becomes empty, the corresponding BST node should be removed as well.</li>

 <li>The mode is the value in the BSTHeapTree that occurs most frequently. In the example the mode is 13 (node marked in green).</li>

</ol>

Your class should include the following methods:

<ul>

 <li>int add (E item) – returns the number of occurrences of the item after insertion</li>

 <li>int remove (E item) – returns the number of occurrences of the item after removal</li>

 <li>int find (E) – returns the number of occurrences of the item in the BSTHeapTree</li>

 <li>find_mode ()</li>

</ul>

Test your implementation as follows:

<ol>

 <li>Insert the 3000 numbers that are randomly generated in the range 0-5000 into the BSTHeapTree. Store these numbers in an array as well. Sort the numbers to find the number occurrences of all the numbers.</li>

 <li>Search for 100 numbers in the array and 10 numbers not in the array and make sure that the number of occurrences is correct.</li>

 <li>Find the mode of the BSTHeapTree. Check whether the mode value is correct.</li>

 <li>Remove 100 numbers in the array and 10 numbers not in the array and make sure that the number of occurrences after removal is correct.</li>

</ol>




<strong><u>PART 3:</u></strong>

Analyze the time complexity (in most appropriate asymptotic notation) of all methods in your implementation. Attach the code just before its analysis.


