## Big O: Analysis of Algorithm Efficiency
which we often refer to as Space and Time. In order to analyze these limiting factors, we should consider 4 Key Areas for analysis:
* Input Size
* Units of Measurement
* Orders of Growth
* Best Case, Worst Case, and Average Case

************************************************************************


![images (1)](https://user-images.githubusercontent.com/98957434/159837590-f251adb2-2191-482b-9ba4-66b7b39ba569.png)

## Linked Lists
A Linked List is a sequence of Nodes that are connected/linked to each other.
The most defining feature of a Linked List is that each Node references the next Node in the link.
There are two types of Linked List - Singly and Doubly.

### Terminology:
- Linked List
- Singly
- Doubly
- Node
- Next
- Head
- Current  

### Types of Linked List:
* Singly Linked List
* Doubly Linked List
* Circular Linked List

### complexity:
* time: O(n) (worse case) the node which has the value that searches for it is last

* space: O(1) This because there is no additional space being used

### what makes arrays and linked lists different?:
### Memory management
- arrays: are static data structures.
- linked lists: are dynamic data structures.
- The biggest differentiator between arrays and linked lists is the way that they use memory in our machines.
- When an array is created, it needs a certain amount of memory(all in one place ). On the other hand, when a linked list is born, it doesn’t need bytes of memory all in one place. One byte could live somewhere, while the next byte could be stored in another place in memory altogether!