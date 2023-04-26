# singly_linked_list

Linked List can be defined as collection of objects called nodes that are randomly stored in the memory.
A node contains two fields i.e. data stored at that particular address and the pointer which contains the address of the next node in the memory.
The last node of the list contains pointer to the null.
![image](https://user-images.githubusercontent.com/126075191/234509925-305d8137-67f7-42be-baf3-71e28b404289.png)
Why use linked list over array?
Better use of Memory: From a memory allocation point of view, linked lists are more efficient than arrays. Unlike arrays, the size for a linked list is not pre-defined, allowing the linked list to increase or decrease in size as the program runs.
Fast Insertion/Deletion Time: Inserting a new node to the beginning or end of a linked list takes constant time (O(1)) as the only steps are to initialize a new node and then update the pointers. Likewise, if there were a tail pointer (similar to the head pointer) insertion to the end of the linked list would also be O(1). Similarly, deletion of the nodes at the beginning and end of the linked list take constant time while deleting a node in the middle of the linked list takes linear time.
Algorithm :
Create a structure node that has two members, one is info that is used to store the data items and another is next field that store the address of next node in the list.

Create starting pointer of the structure datatype.

Create a node, use the malloc function to dynamically allocate memory for the new node.

After creating the node, store the new item in the node using a pointer to that node.

 newnode1->data=2;  // newnode1 accessing the data variable of struct node.
 newnode1->next=newnode2; // Address of next node stored in variable next of struct node.
Create function display , containing temp pointer pointing at the start node and further temp updates to new address.

   struct node *temp;
   temp=start;
   temp=temp->next; // address of next stored in temp
   <img width="662" alt="singly_linked_list" src="https://user-images.githubusercontent.com/126075191/234510221-776ec732-87e6-4cb6-998c-0dd60424c8da.PNG">
Linked List Applications
Dynamic memory allocation
Implemented in stack and queue
In undo functionality of softwares
Hash tables, Graphs
