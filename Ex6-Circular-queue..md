# Ex6 Dequeue Elements from Circular Queue
## DATE:28-4-2025
## AIM:
To write a C program to delete three elements from the filled circular queue.

## Algorithm
1.Check if the queue is empty 
2.Store the element to be dequeued 
3.Increment the front index 
4.Check if the queue became empty  
5.Return the dequeued element   

## Program:
```
/*
Program to delete three elements from the filled circular queue
Developed by:Divya R V 
RegisterNumber: 212223100005 
*/
```
```
/*#include <stdio.h>

#define SIZE 5

int items[SIZE];
int front = -1, rear = -1;
*/
int deQueue() {
  int element;
if(isEmpty())

{
    printf("Queue is empty !!\n");
    return (-1);
}else{
    element=items[front];
    if(front==rear){
        front=-1;
        rear=-1;
    }
    else{
        front=(front+1) %SIZE;
        
    }
    return (element);
}
}
```
## Output:

![Screenshot 2025-04-29 091915](https://github.com/user-attachments/assets/1cbbcb42-4acf-4a79-9011-82122f2f0265)


## Result:
Thus, the C program to delete three elements from the filled circular queue is implemented successfully.
