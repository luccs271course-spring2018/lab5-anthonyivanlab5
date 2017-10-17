# Questions

**Question 1**

*(Why does `LinkedStack` not require an explicit constructor?)*

- It does not require a constructor because any new stack starts as empty and does not need any arguments to be created.

**Question 2**

*(What is the time and (extra) space complexity of each of the `LinkedStack` methods, as well as `ReverseLines.main`?)*

- The LinkedStack methods are of complexity O(1), except for asList(), which is O(n). The ReverseLines main is O(n).

**Question 3**

*(How else (not using `Node`) could we have implemented `LinkedStack` in such a way that it is still based on a linked list but the `asList` method uses constant time and space?)*

- We could have preallocated space for the elements and stored the stack in an array.

**Question 4**

*(Is it better for `push` and `pop` to return the item or the stack itself? Briefly discuss the pros and cons of each design.)*

- *Push/Pop*
- Pro: It, specifically in the case of `pop`, is the easiest and more direct way to manipulate and use an element retrieved from the stack (and saves memory).
- Con: It takes an extra step to utilize the whole stack after adding/removing, as opposed to running the method and getting the whole stack in return to be used.
- *Stack*
- Pro: Allows quicker access to the entire stack after pushing or popping a new element.
- Cons: Makes retrieving a removed/popped element more complicated.