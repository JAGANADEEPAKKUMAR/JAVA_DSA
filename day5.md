# SEARCH AN ELEMENT IN LINKED LIST
- To `search for an element` in a linked list, the process involves traversing the linked list from the beginning (the head node) to the end, checking each node's data to see if it matches the target value. 

```
Node temp = head;
while (temp != null) {
    if (temp.data == val) {
                return true; // Return true if value is found
    }
    temp = temp.next;
}
return false; 
```
## Steps to Search an Element in a Linked List
1. <b>Start from the Head:</b>

    - Begin the search at the head node of the linked list.
2. <b>Compare Node Data:</b>

    - Compare the data stored in the current node with the target value.
3. <b>Move to the Next Node:</b>

    - If the data of the current node does not match the target value, move to the next node using the next pointer.
4. <b>Repeat Until the End:</b>

    - Continue this process for each node in the linked list.
5. <b>Check for the Target:</b>

    - If the target value is found, return the position of the node or confirm its presence.
    - If the end of the linked list is reached without finding the value, conclude that the element is not in the list.

### Example of Searching in a Linked List
Let's consider the following linked list:

<b>10 -> 20 -> 30 -> 40 -> None</b>

- To search for the element `30`:
    1. Start at the head node (`10`).
    2. Compare `10` with `30` → Not a match → Move to the next node.
    3. Compare `20` with `30` → Not a match → Move to the next node.
    4. Compare `30` with `30` → Match found → Return the position or success message.


## Time Complexity
- <b>Traversal:</b> The linked list is traversed node by node.
- <b>Worst-case Time Complexity:</b>𝑂(𝑛), where n is the number of nodes in the list. This happens if the element is at the end or not present.
## Space Complexity
- 𝑂(1), as no extra space is required other than a pointer for traversal.

