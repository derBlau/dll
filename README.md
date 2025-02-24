# Doubly Linked List


## Task requirements

Hide the fields of the struct by making the LinkedList **struct opaque**

The link list should keep track of its length -> another struct for the linked list itself as well as any other data

**Prefix all functions created to implement the below with the prefix bleu_ll_ - eg: bleu_ll_new.** In general when making functions in C for libraries or some component of your program that are accessible from other areas, you give them a prefix so that if something needs to use a bunch of different libraries or whatever, you don't have name collisions.

Need a way to construct a new linked list - To do this, create a function that lets you initialize a new linked list struct with the following signature _LinkedList* (void)_. **This function should dynamically allocate a new LinkedList**

Need a way to free  the linked list and its nodes - To do this, have a function with the following signature void `(LinkedList**)` The reason why this is a pointer to a pointer is so that you can set the `LinkedList*` to `NULL` when its done preventing a dangling reference from being used

All the linked list functions below should start with a `LinkedList*` argument and have other args after the linked list arg. Return types are according to what the fn's do. For the first function below, an example is given.

- Have function to get pointer to first node, should **run in constant time** - This one should be along the lines of `LinkedListNode* bleu_ll_get_first_node()`

- Have function to get pointer to last node, should run in constant time

- Have function to get first element, should run in constant time - The element would be `int`, not `LinkedListNode*`.

- Have function to get last element, should run in constant time

- Have function to get current length of linked list, should run in constant time

- Have function to get the nth node of the linked list, should **run in linear time**

- Have function to get the nth element of the linked list, should run in linear time

- Have function to clear linked list, should run in linear time

- Have function to add to front of linked list, should run in constant time

- Have function to add to back of linked list, should run in constant time

- Have function to add node at nth index of the linked list and shift current elements from then on up, should run in linear time

- Have function to remove the first node, return its value, should run in constant time

- Have function to remove the last node, return its value, should run in constant time

- Have function to remove the nth node, should run in linear time

- Have function to find the first element from the beginning with a particular value, should run in linear time

- Have function to find the first element from the end going backwards with a particular value, should run in linear time

- Have function to find the first node from the beginning with a particular node value, should run in linear time

- Have function to find the first node from the end going backwards with a particular node value, should run in linear time
 
- Have function to swap the n'th node with the m'th node, should run in linear time

- Have function to merge two linked lists together (merging linked list a and b will result in elements from a first then b) - free linked list b and return a pointer to linked list a out - should run in linear time

*Optional functions (these are harder)*

- Have function to sort linked list

- Have function to take out any duplicate elements in the linked list

- Have function to get element in node - eg: `int bleu_ll_node_get_value(LinkedListNode *node)`

- Have function to get next node

- Have function to get prev node

*Additionally, nodes within linked lists should have the following functions prefixed with bleu_ll_node_, starting with a `LinkedListNode*` argument*
