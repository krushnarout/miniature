## [Flattening a Linked List](https://www.geeksforgeeks.org/problems/flattening-a-linked-list/1)

Given a Linked List, where every node represents a sub-linked-list and contains two pointers:

(i) a next pointer to the next node,

(ii) a bottom pointer to a linked list where this node is head.

Each of the sub-linked lists is in sorted order.

Flatten the Link List so all the nodes appear in a single level while maintaining the sorted order.

Note: The flattened list will be printed using the bottom pointer instead of the next pointer. Look at the printList() function in the driver code for more clarity.

### Examples:

Input:

![blobid0_1722066129](https://github.com/user-attachments/assets/fa2aa1fd-9535-4459-8fba-16065459bbdc)

```
Output:  5-> 7-> 8- > 10 -> 19-> 20-> 22-> 28-> 30-> 35-> 40-> 45-> 50.
Explanation: The resultant linked lists has every node in a single level.(Note: | represents the bottom pointer.)
```

Input:

![blobid1_1722066171](https://github.com/user-attachments/assets/ebb6793a-6b64-4a91-8784-c71c1b2d5b31)

```
Output: 5-> 7-> 8-> 10-> 19-> 22-> 28-> 30-> 50
Explanation: The resultant linked lists has every node in a single level.(Note: | represents the bottom pointer.)
```

Note: In the output section of the above examples, the -> represents the bottom pointer.

**Expected Time Complexity:** O(n * n * m)

**Expected Auxiliary Space:** O(n)

### Constraints:

- 0 <= number of nodes <= 50
- 1 <= no. of nodes in sub-LinkesList(mi) <= 20
- 1 <= node->data <= 10^3
