# Ex9 Applications of Queue - SJF
## DATE:28-4-2025
## AIM:
To incorporate the code to calculate the Total Waiting Time and Average Waiting Time in Shortest Job First scheduling algorithm.
## Algorithm
1.Input and Initialization 
2.Sort Processes 
3. Calculate Waiting Time 
4. Calculate Total Waiting Time 
5. Calculate Average Waiting Time   

## Program:
```
/*
Program to find the Total Waiting Time and Average Waiting Time in Shortest Job First scheduling algorithm.
Developed by:Divya R V 
RegisterNumber: 212223100005 
*/
```
```
#include<stdio.h>
 
int main()
{
    int bt[20],p[20],wt[20],tat[20],i,j,n,total_tat=0,total_wt=0,pos,temp;
    scanf("%d",&n);
    for(i=0;i<n;i++)
    {
        scanf("%d",&bt[i]);
        p[i]=i+1;
    }
    for(i=0;i<n;i++)
    {
        pos=i;
        for(j=i+1;j<n;j++)
        {
            if(bt[j]<bt[pos])
            
            {
                pos=j;
            }
        }
        if(i!=pos)
        {
            temp=bt[i];
            bt[i]=bt[pos];
            bt[pos]=temp;
            temp=p[i];
            p[i]=p[pos];
            p[pos]=temp;
        }
    }
    wt[0]=0;        
    for(i=1;i<n;i++)
    {
        wt[i]=wt[i-1]+bt[i-1];
        total_wt+=wt[i];
    }
    for(i=0;i<n;i++)
    {
        tat[i]=bt[i]+wt[i];     //calculate turnaround time
        total_tat+=tat[i];
    }
    printf("Process    Burst Time    Waiting Time  Turnaround Time\n");
    for(i=0;i<n;i++)
    {
        printf("p%d          %d               %d             %d\n",p[i],bt[i],wt[i],tat[i]);
    }
    printf("Average Waiting Time=%f\n",(float)total_wt/n);
    printf("Average Turnaround Time=%f\n",(float)total_tat/n);
 
   
}

```
## Output:

![Screenshot 2025-04-29 093222](https://github.com/user-attachments/assets/9424062a-5c13-4783-984b-d4484690855e)


## Result:
Thus, the code to calculate the Total Waiting Time and Average Waiting Time in Shortest Job First scheduling algorithm is implemented successfully.
