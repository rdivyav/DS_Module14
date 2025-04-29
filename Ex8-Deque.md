# Ex8 Deque
## DATE: 28-4-2025
## AIM:
To write a C function to count the number of elements present in the deque.

## Algorithm
1. Initialization
2. Check for Empty Deque  
3.Calculate the Count (Circular Array) 
4.Calculate the Count (Linked List)  
5.Return the Count   

## Program:
```
/*
Program to count the number of elements present in the deque
Developed by:Divya R V 
RegisterNumber: 212223100005 
*/
```
```
int count(int *arr) {
  int c = 0, i;

  for (i = 0; i < MAX; i++) {
    if (arr[i] != 0)
      c++;
  }
  return c;
}
```
## Output:

![Screenshot 2025-04-29 092852](https://github.com/user-attachments/assets/38fc0f2f-3b87-4034-aa60-fea4a4179c7a)


## Result:
Thus, the C code to count the number of elements present in the deque is implemented successfully.
