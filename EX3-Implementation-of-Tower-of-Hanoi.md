# EX3 Implementation of Tower of Hanoi
## DATE:
02-06-2025
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm
1 . Start the program.

2 . Define a recursive function towerOfHanoi(n, source, auxiliary, destination).

3 . If n == 1, print the move from source to destination and return.

4 . Recursively move n-1 disks from source to auxiliary using destination as intermediate.

5 . Move the nth disk from source to destination.

6 . Recursively move n-1 disks from auxiliary to destination using source as intermediate.

7 . End the program.

## Program:
```
/*
Program to implement Tower of Hanoi
Developed by: 
RegisterNumber:  
*/

#include<stdio.h> 
void TOH(int n,char x,char y,char z) 
  { 
    if(n>0) { 
      TOH(n-1,x,z,y); 
      printf("%c to %c",x,y); 
      printf("\n"); 
      TOH(n-1,z,y,x); 
    } 
} 
int main() 
{ 
  int n=2; 
  TOH(n,'A','B','C'); 
}
```


## Output:
![image](https://github.com/user-attachments/assets/79cb0326-4488-4cbe-8df4-eb5623dd74dd)


## Result:
Thus, the C program to implement Tower of Hanoi using recursion is implemented successfully.
