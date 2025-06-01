# EX 1D Linear search
## DATE: 29-04-2025
## AIM:
To write a python program for a search function with parameter list name and the value to be searched using string values.


## Algorithm
1. Start the program.
2. Define a function search(List, n).
3. Take input for the number of elements x in the list.
4. Read x string values from the user and store them in the list List.
5. Take input for the string value n to be searched.
5. Call the search(List, n) function to check and print the result.
6. End the program.  

## Program:
```
/*
Program to implement a search function with parameter list name and the value to be searched using string values.
Developed by: Vishinu H
Register Number: 212223220124  
*/

def search(List, n):
    if n in List:
        print("Found")
    else:
        print("Not Found")
        
x = int(input())
List = [input() for i in range(x)]
n = input()
```

## Output:
![image](https://github.com/user-attachments/assets/be2a9f5a-09c1-4fe4-b88c-6e412702483c)


## Result:
The program was executed successfully, and it correctly checks if the input element is present in the list, printing "Found" if the element exists or "Not Found" if it does not.
