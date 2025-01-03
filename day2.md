# CONVERTING ARRAY TO LINKED LIST

- To convert an array to a linked list in programming, you essentially need to iterate through the array and create a node for each element, linking the nodes together. 
- Here is the code in java to convert an array to linked list.

```
public class LinkedList{
    private static Node convertArr2LL(int[] arr)
    {
        Node head = new Node(arr[0]);
        Node mover = head;
        for(int i = 1;i < arr.length; i++){
            Node temp = new Node(arr[i]);
            mover.next = temp;
            mover = temp;
        }
        return head;
    }
    public static void main(String[] args){
        int[] arr = {12,5,6,8};
        Node head = convertArr2LL(arr);
        System.out.println(head.data);
    }
}

```
- The TIME COMPLEXITY is O(N).

## EXPLANATION

1. <b>Purpose:</b> The LinkedList class includes a method convertArr2LL that converts an integer array into a singly linked list, with each array element becoming a node.

2. <b>Node Creation:</b> The method initializes the head of the linked list using the first element of the array, then iteratively creates and links nodes for the remaining elements.

3. <b>Traversal Pointer:</b> A pointer (mover) is used to traverse the list while creating and linking new nodes.

4. <b>Main Method:</b> The main method creates an array, calls convertArr2LL to generate the linked list, and prints the data of the head node.

5. <b>Output:</b> For the input array {12, 5, 6, 8}, the program constructs a linked list and outputs 12, the first element.