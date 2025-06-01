# EX 1A Reverse a String
## DATE: 29-04-2025
## AIM:
To write a program to create a recursive function to reverse a string.

## Algorithm
1. Start the program.
2. Define a recursive function rev(s):
3. Accept a string input from the user and store it in variable s.
4. Call the function rev(s) and print the returned reversed string.
5. End the program.

## Program:
```
Python program to create a recursive function to reverse a string.
Name: Vishinu H
Reg No: 212223220124

def rev(s):
    if len(s)==0:
        return s
    else:
        return s[-1] + rev(s[:-1])
        
s= input()
print(rev(s))
```

## Output:
![image](https://github.com/user-attachments/assets/3541890e-bd12-43b9-a754-960f9d30b9e6)



## Result:
The program successfully reverses the input string using recursion. When the user provides an input string, the output displays the reversed version of the string
