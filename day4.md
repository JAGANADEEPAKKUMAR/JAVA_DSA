# LENGTH OF A LINKED LIST
The length of a linked list is the total number of nodes present in the list. You can calculate the length by traversing the list from the head (starting node) to the end (where the `next` pointer is `null`), while counting the nodes.
## Algorithm to Find the Length of a Linked List:
1. Initialize a variable `count` to `0` to store the number of nodes.
2. Start from the head node.
3. Traverse through the linked list:
    - Increment the count for each node.
    -  Move to the next node using the next pointer.
4. Stop when the next pointer is null.
5. The value of count is the length of the linked list.
### CODE SNIPPET(JAVA)
```
int count = 0;
while (temp != null) {
    count++;
    temp = temp.next;
}
System.out.println(count);
```
### Explanation of Each Line:
1. `int count = 0;`

    - This initializes the variable `count` to `0`. It will store the total number of nodes in the linked list.
2. `while (temp != null)`

    - This loop runs as long as `temp` is not `null`.
    - `temp` is a reference to the current node in the linked list, typically starting at the `head` node.
3. `count++;`

    - Each time a node is encountered, the `count` is incremented by `1`.
4. `temp = temp.next;`

    - After processing the current node, this moves the `temp` pointer to the `next` node in the list.
    - If the `next` pointer is `null` (end of the list), the loop stops.
5. `System.out.println(count);`

    - After the loop finishes, the `count` variable contains the total number of nodes in the linked list.
    - This line prints the value of `count`, which is the <b>length of the linked list.</b>
