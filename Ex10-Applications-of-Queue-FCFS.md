# Ex10 Applications of Queue – FCFS
## DATE:28-4-2025
## AIM:
To write a C function to calculate the turnaround time of each process given their burst time and waiting time in First Come first Serve scheduling algorithm.
## Algorithm
1. Initialization
2. Calculating Waiting Time
3.  Calculating Turnaround Time
4. Calculating Total Times 
5. Displaying Results  

## Program:
```
/*
Program to find and display the priority of the operator in the given Postfix expression
Developed by:Divya R V 
RegisterNumber:212223100005  
*/
```
```
/*#include <stdio.h>*/
void turnaroundtime( int proc[20], int n,int burst_time[20], int wait_time[20], int tat[20])
{
   // calculating turnaround time by adding
   // burst_time[i] + wait_time[i]
   int i;
   //type your code here...
   for(i=0;i<n;i++)
   {
       tat[i]=wait_time[i]+burst_time[i];
       
   }
   
}
```
## Output:

![Screenshot 2025-04-29 093633](https://github.com/user-attachments/assets/b3184a6e-1ef3-425d-bac4-23172e3c3ffc)


## Result:
Thus, the C function to calculate the turnaround time of each process given their burst time and waiting time in First Come first Serve scheduling algorithm is implemented successfully.
