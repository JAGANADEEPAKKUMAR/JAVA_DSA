# TRAVERSAL OF LINKED LISTS
```
    2   --->    3   --->    1   --->    8   --->    NULL
```
## SINGLY LINKED LIST TRAVERSAL

1. <b>Definition:</b> A singly linked list contains nodes with two fields:
- `data`: stores the value of the node.
- `next`: points to the next node in the list.

2. <b>Steps:</b>
- Start at the head of the list.
- While the current node is not `NULL`:
- Print the data of the current node.
- Move to the next node by updating the current node to the value of `next`.

### CODE SNIPPET(JAVA)

```
Node temp = head;
while(temp != null){
    System.out.print(temp.data + " ");
    temp = temp.next;
}
```
1. <b>Initialization</b>(`Node temp = head;`):
- We initialize a temporary pointer `temp` to the `head` of the list.
- This allows us to traverse the list without modifying the original head pointer.
2. <b>Condition</b>(`temp != null):
- We check if the current node `temp` is not `NULL`.
- If it's not `NULL`, we proceed to print the data and move to the next node.
3. <b>Printing Data</b>(`System.out.print(temp.data + " ");`
- We print the data of the current node `temp`.
4. <b>Moving to Next Node</b>(`temp = temp.next;`):
- We update the `temp` pointer to point to the next node in the list by assigning the value of `next` to `temp`.